<script>
    // 1. Smooth Reveal Animation
    document.addEventListener('DOMContentLoaded', () => {
        const card = document.querySelector('.portfolio-card');
        card.style.opacity = '0';
        card.style.transform = 'scale(0.95) translateY(20px)';
        card.style.transition = 'all 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275)';

        setTimeout(() => {
            card.style.opacity = '1';
            card.style.transform = 'scale(1) translateY(0)';
        }, 200);
    });

    // 2. Interactive "Vibe" for Work Showcase
    const images = document.querySelectorAll('.work-grid img');
    images.forEach(img => {
        img.addEventListener('mouseenter', () => {
            img.style.transform = 'scale(1.05)';
            img.style.filter = 'brightness(1.1)';
        });
        img.addEventListener('mouseleave', () => {
            img.style.transform = 'scale(1)';
            img.style.filter = 'brightness(1)';
        });
    });

    // 3. Simple Haptic-Style Click Feedback
    const buttons = document.querySelectorAll('.btn');
    buttons.forEach(btn => {
        btn.addEventListener('touchstart', () => {
            btn.style.transform = 'scale(0.96)';
        });
        btn.addEventListener('touchend', () => {
            btn.style.transform = 'scale(1)';
        });
    });

    // 4. "Share Portfolio" Logic
    function sharePortfolio() {
        if (navigator.share) {
            navigator.share({
                title: 'CEO Ddamulira Fahim - HIMI VISUALS',
                text: 'Check out my digital portfolio for professional videography and photography.',
                url: window.location.href
            }).then(() => console.log('Successful share'))
              .catch((error) => console.log('Error sharing', error));
        } else {
            alert("Copy this link to share: " + window.location.href);
        }
    }
</script>
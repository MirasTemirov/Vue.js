<template>
  <div class="photo-container">
    <!-- Левый столбец -->
    <div class="column">
      <div class="photo-item">
        <img :src="imagePath" alt="KBTU" />
        <div class="photo-info">
          <p class="photo-title">The AI magically removes moving objects from videos.</p>
          <p class="photo-date">July 19, 2019</p>
        </div>
      </div>
      <div class="photo-item">
        <img :src="imagePath" alt="KBTU" />
        <div class="photo-info">
          <p class="photo-title">The AI magically removes moving objects from videos.</p>
          <p class="photo-date">July 19, 2019</p>
        </div>
      </div>
    </div>

    <!-- Центральный элемент -->
    <div class="column center-column">
      <div class="photo-item tall-photo">
        <img :src="imagePath" alt="KBTU" />
        <div class="photo-info">
          <p class="photo-title">The AI magically removes moving objects from videos.</p>
          <p class="photo-date">July 19, 2019</p>
          <!-- Добавляем два слова с рамками -->
          <div class="tags">
            <span class="tag red">Study</span>
            <span class="tag blue">Diplom</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Правый столбец -->
    <div class="column">
      <div class="photo-item">
        <img :src="imagePath" alt="KBTU" />
        <div class="photo-info">
          <p class="photo-title">The 20 Biggest Fintech Companies In America 2019</p>
          <p class="photo-date">July 19, 2019</p>
        </div>
      </div>
      <div class="photo-item">
        <img :src="imagePath" alt="KBTU" />
        <div class="photo-info">
          <p class="photo-title">The 20 Biggest Fintech Companies In America 2019</p>
          <p class="photo-date">July 19, 2019</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import imagePath from '@/assets/кбту.jpg'; // Убедитесь, что путь правильный
</script>

<style scoped>
.photo-container {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: 20px;
  padding: 20px;
  max-width: 100%;
  box-sizing: border-box;
  margin: 0 auto;
}

.column {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.center-column {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.photo-item {
  position: relative;
  width: 300px;
  height: 200px;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s, box-shadow 0.3s;
}

.photo-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.photo-item:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
}

.photo-info {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: 10px;
  background: rgba(0, 0, 0, 0.6);
  color: white;
}

.photo-title {
  font-size: 1.2rem;
  margin: 0 0 5px 0;
}

.photo-date {
  font-size: 0.9rem;
  margin: 0;
}

.tags {
  margin-top: 10px; 
}

.tag {
  display: inline-block; 
  margin-right: 5px; 
  padding: 3px 8px; 
  border-radius: 5px; 
  font-size: 0.8rem; 
  color: white; 
}

.red {
  background-color: #534dff; 
  border: 1px solid #3300ff; 
}

.blue {
  background-color: #ff4db8; 
  border: 1px solid #ff00d4; 
}

.tall-photo {
  width: 300px;
  height: 420px;
}
</style>

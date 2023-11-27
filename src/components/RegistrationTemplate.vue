<template>
  <section class="form-sec-cntr">
    <h5>Join Prezent and transform the way your team Collaborates, Creates and Presents.</h5>

    <div class="form-cntr">
      <form>
        <input type="text" placeholder="First Name" />

        <input type="text" placeholder="Last Name" />

        <input type="text" placeholder="Work Email" />

        <input type="text" placeholder="Company Name" />

        <select>
          <option value="" disabled selected hidden>Company Size</option>
          <option>less than 100</option>
          <option>between 100-1000</option>
          <option>more than 1000</option>
        </select>

        <input type="number" placeholder="Phone" />

        <input type="submit" value="Continue" />
      </form>
    </div>
  </section>
</template>

<style scoped>
.form-sec-cntr h5 {
  color: white;
  font-size: 1rem;
  font-weight: 600;
  margin-top: 1rem;
}

.form-cntr {
  margin-top: 3rem;
}

.form-cntr form {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

form input[type='text'],
form input[type='number'],
form select {
  width: 100%;
  padding: 1rem 0.5rem;
  color: white;
  font-size: 1rem;
  font-weight: 500;
  background-color: transparent;
  border: transparent;
  border-bottom: 1px solid #ffffff40;
}

form input {
  outline: none;
}

::placeholder {
  color: #ffffff8f;
  font-size: 0.95rem;
  font-weight: 500;
}

form select {
  outline: none;
}

form input[type='submit'] {
  width: 150px;
  font-size: 1.2rem;
  padding: 0.75rem 1rem;
  border-radius: 30px;
  border: none;
  color: #1075ab;
}

@media (max-width: 768px) {
  .form-sec-cntr h5 {
    color: black;
    margin-top: 1rem;
    font-weight: 600;
  }
  .form-cntr {
    background-color: #1075ab;
    padding: 1rem;
    border-radius: 15px;
    margin-top: 2rem;
  }
}
</style>

<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-5 offset-sm-1">
        <h1 class="section__title">Contact</h1>
        <h2 class="section__lead">Send me a message</h2>

        <p>
          For more detailed information on how I can help you achieve your goals, let me know how to reach
          you and I will get back to you within two working days.
        </p>

        <follow-me />
      </div>
      <div class="col-sm-6">
        <form action="">
          
          <div class="form-group">
            <label class="form-label" for="">Full name</label>
            <input type="text" class="form-control" name="name" maxlength="50" required />
          </div>

          <div class="form-group">
            <label class="form-label" for="">Country</label>
            <input type="text" class="form-control" name="country" maxlength="30" required />
          </div>

          <div class="form-group">
            <label class="form-label" for="">Email</label>
            <input type="email" class="form-control" name="email" maxlength="30" required />
          </div>

          <div class="form-group">
            <label class="form-label" for="">Phone</label>
            <input type="tel" class="form-control" name="tel" maxlength="30" required />
          </div>

          <div class="form-group">
            <label class="form-label" for="">Telegram (optional)</label>
            <textarea class="form-control" name="telegram"></textarea>
          </div>

          <button type="submit" class="btn btn-primary">
            Done
          </button>

        </form>
      </div>
    </div>

  </div>
</template>

<script>
import FollowMe from '@/components/FollowMe'
export default {
  name: 'ContactSection',
  components: {
    FollowMe
  }
}
</script>
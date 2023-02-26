<template>
    <!-- Success Modal Newsletter -->
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">

                <!-- Modal header -->
                <div class="modal-header">
                    <h1 class="modal-title fs-5" id="exampleModalLabel">Thanks!</h1>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>

                <!-- Modal body -->
                <div class="modal-body d-flex align-items-center">
                    <i class="ri-mail-line me-3"></i> E-mail subscribed with success!
                </div>

                <!-- Modal footer -->
                <div class="modal-footer">
                    <button type="button" class="btn btn-success" data-bs-dismiss="modal">Ok</button>
                </div>
            </div>
        </div>
    </div>

    <div class="footer mt-5">
        <footer class="container pt-4 pb-2 mx-auto">
            <div class="row d-flex justify-content-between">
                <div class="col-6 col-md-2 mb-3">
                    <h5>Section</h5>
                    <ul class="nav flex-column">
                        <li class="nav-item mb-2">
                            <RouterLink class="nav-link p-0 text-muted" to="/">
                                Home
                            </RouterLink>
                        </li>
                        <li class="nav-item mb-2">
                            <RouterLink class="nav-link p-0 text-muted" to="/reviews">
                                Reviews
                            </RouterLink>
                        </li>
                        <li class="nav-item mb-2">
                            <RouterLink class="nav-link p-0 text-muted" to="/about">
                                About
                            </RouterLink>
                        </li>
                    </ul>
                </div>

                <div class="col-md-5 offset-md-1 mb-3">
                    <form>
                        <h5>Subscribe to our newsletter!</h5>
                        <p>Monthly reviews of animes directly to your e-mail</p>
                        <div class="d-flex flex-column flex-sm-row w-100 gap-2">
                            <label for="newsletter1" class="visually-hidden">Email address</label>
                            <input id="newsletter1" type="email" class="form-control" placeholder="Email address">
                            <button class="btn btn-primary" type="button" data-bs-toggle="modal"
                                data-bs-target="#exampleModal">Subscribe</button>
                        </div>
                    </form>
                </div>
            </div>

            <div class="d-flex flex-column flex-sm-row justify-content-between pt-4 my-3 border-top">
                <p>&copy; {{ new Date().getFullYear() }} Anime Rating, Inc. All rights reserved.</p>
                <ul class="list-unstyled d-flex justify-content-center">
                    <li class="ms-3">
                        <a class="link-dark text-decoration-none" href="https://instagram.com">
                            <h5><i class="ri-instagram-line"></i></h5>
                        </a>
                    </li>
                    <li class="ms-3">
                        <a class="link-dark text-decoration-none" href="https://facebook.com">
                            <h5><i class="ri-facebook-fill"></i></h5>
                        </a>
                    </li>
                    <li class="ms-3">
                        <a class="link-dark text-decoration-none" href="https://youtube.com">
                            <h5><i class="ri-youtube-line"></i></h5>
                        </a>
                    </li>
                </ul>
            </div>
        </footer>
    </div>
</template>

<style scoped>
.footer {
    border-top: 3px solid #198754;
}
</style>
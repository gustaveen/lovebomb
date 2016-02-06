## Proposed BEM structure

    /*If extra wrappers are needed use &__content or &__container */

    .site
        &__content | &--no-section
        &__section
            &__section-header
                &__section-title
                &__section-link

    .header-main
        &__content | &--tight
            &__branding
                &__logo-link
                &__logo
                &__logo-text
            &__menu-main | navbar

    .navbar
        &__content
            &__item | &--current
                &__link | &--large | &--tight

    .searchform


    .mobile-menu
        &__content

    .hero (wrapper för "heroyta" inget passande namn)
        &__menu | .main-entry

    .hero | --large
        &__content
            &__caption
                &__title
                &__taglin
                &__link

    .quick-menu
        &__item
            &__link
                &__title
                &__description
                (&__icon)

    .feed
        &__content
            &__item | --small | --large
                &__link
                    &__item-date
                    &__item-title | --small | --large
                    &__item-excerpt

    .article

    .sidebar
        &__title
        &__menu | .js-sidebar-menu
            &__menu-item | --parent | --current
                &__menu-link | --primary | --secondary



    .blurbs
        &__item
            &__link
                &__item-description
                &__item-title

    .footer
        &__content


### Grid

    /* Using Fröjd default grid, write class in markup */
    .u-g-6-12 | --s | --m | --l | --xl

    /* Table grid */
    .u-tg-6-12 | --s | --m | --l | --xl


### Icons
    /* For svg background images, use the mixin #m-svg-icon({filename}, {background-size(optional)});
    Example for icon-search.svg: */

    #m-svg-icon(icon-search);
    #m-svg-icon(icon-search, 15px 18px);
    #m-svg-icon(icon-search, contain);

    /* Urls */
    @url--image: '../../builds/img/';



### Media Queries

    /* Media querys used, only for quick copy paste stub */
    @media @media--s {

    }

    @media @media--m {

    }

    @media @media--l {

    }

    @media @media--xxl {

    }

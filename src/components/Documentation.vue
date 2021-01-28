 <template>

          <!-- Page title -->
          <div class="page-header d-print-none">
            <div class="row align-items-center">
              <div class="col">
                <h2 class="page-title">
                  Documentation
                </h2>
              </div>
            </div>
          </div>
          <div class="row">
            <div class="d-none d-lg-block col-lg-3">
              <ul class="nav nav-vertical">
                <li class="nav-item">
                  <a href="#menu-base" class="nav-link" data-bs-toggle="collapse" aria-expanded="true">
                    <span class="nav-link-icon"><svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M8 9l3 3l-3 3" /><line x1="13" y1="15" x2="16" y2="15" /><rect x="4" y="4" width="16" height="16" rx="4" /></svg>
                    </span>
                    Getting started
                    <span class="nav-link-toggle"></span>
                  </a>
                  <ul class="nav nav-pills collapse show" id="menu-base">
                    <li class="nav-item">
                     <!-- <a href="../docs/index.html" class="nav-link active">-->
                      <router-link to="/Documentation" class="nav-link">Introduction</router-link>
                          <!--  Introduction-->
                      <!--  </a>-->
                    </li>
                    <li class="nav-item">
                     <!--<a href="../docs/usage.html" class="nav-link">-->
                     <router-link to="../components/Card1_Apex.vue" class="nav-link">Usage</router-link>                  
                        <!-- Usage-->
                        <!--  </a>-->
                    </li>
                    <li class="nav-item">
                      <a href="../docs/colors.html" class="nav-link">
                        Colors
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/typography.html" class="nav-link">
                        Typography
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/icons.html" class="nav-link">
                        Icons
                      </a>
                    </li>
                  </ul>
                </li>
                <li class="nav-item">
                  <a href="#menu-components" class="nav-link" data-bs-toggle="collapse" aria-expanded="false">
                    <span class="nav-link-icon"><svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 7h3a1 1 0 0 0 1 -1v-1a2 2 0 0 1 4 0v1a1 1 0 0 0 1 1h3a1 1 0 0 1 1 1v3a1 1 0 0 0 1 1h1a2 2 0 0 1 0 4h-1a1 1 0 0 0 -1 1v3a1 1 0 0 1 -1 1h-3a1 1 0 0 1 -1 -1v-1a2 2 0 0 0 -4 0v1a1 1 0 0 1 -1 1h-3a1 1 0 0 1 -1 -1v-3a1 1 0 0 1 1 -1h1a2 2 0 0 0 0 -4h-1a1 1 0 0 1 -1 -1v-3a1 1 0 0 1 1 -1" /></svg>
                    </span>
                    Components
                    <span class="nav-link-toggle"></span>
                  </a>
                  <ul class="nav nav-pills collapse" id="menu-components">
                    <li class="nav-item">
                      <a href="../docs/alerts.html" class="nav-link">
                        Alerts
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/avatars.html" class="nav-link">
                        Avatars
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/badges.html" class="nav-link">
                        Badges
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/breadcrumb.html" class="nav-link">
                        Breadcrumb
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/buttons.html" class="nav-link">
                        Buttons
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/cards.html" class="nav-link">
                        Cards
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/carousel.html" class="nav-link">
                        Carousel
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/dropdowns.html" class="nav-link">
                        Dropdowns
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/divider.html" class="nav-link">
                        Divider
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/empty.html" class="nav-link">
                        Empty states
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/form-elements.html" class="nav-link">
                        Form elements
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/form-helpers.html" class="nav-link">
                        Form helpers
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/modals.html" class="nav-link">
                        Modals
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/page-headers.html" class="nav-link">
                        Page headers
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/progress.html" class="nav-link">
                        Progress
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/range-slider.html" class="nav-link">
                        Range slider
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/ribbons.html" class="nav-link">
                        Ribbons
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/skeleton.html" class="nav-link">
                        Skeleton
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/spinners.html" class="nav-link">
                        Spinners
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/steps.html" class="nav-link">
                        Steps
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/switch-icon.html" class="nav-link">
                        Switch icon
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/tables.html" class="nav-link">
                        Tables
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/tabs.html" class="nav-link">
                        Tabs
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/timelines.html" class="nav-link">
                        Timelines
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/toasts.html" class="nav-link">
                        Toasts
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/tooltips.html" class="nav-link">
                        Tooltips
                      </a>
                    </li>
                  </ul>
                </li>
                <li class="nav-item">
                  <a href="#menu-utils" class="nav-link" data-bs-toggle="collapse" aria-expanded="false">
                    <span class="nav-link-icon"><svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M12 12c2 -2.96 0 -7 -1 -8c0 3.038 -1.762 4.383 -2.989 5.642c-1.226 1.26 -2.011 2.598 -2.011 4.358a6 6 0 1 0 12 0c0 -1.532 -.77 -2.94 -1.714 -4c-1.786 3 -3.077 3 -4.286 2z" /></svg>
                    </span>
                    Utilities
                    <span class="nav-link-toggle"></span>
                  </a>
                  <ul class="nav nav-pills collapse" id="menu-utils">
                    <li class="nav-item">
                      <a href="../docs/cursors.html" class="nav-link">
                        Cursors
                      </a>
                    </li>
                  </ul>
                </li>
                <li class="nav-item">
                  <a href="#menu-plugins" class="nav-link" data-bs-toggle="collapse" aria-expanded="false">
                    <span class="nav-link-icon"><svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><rect x="4" y="4" width="6" height="6" rx="1" /><rect x="4" y="14" width="6" height="6" rx="1" /><rect x="14" y="14" width="6" height="6" rx="1" /><line x1="14" y1="7" x2="20" y2="7" /><line x1="17" y1="4" x2="17" y2="10" /></svg>
                    </span>
                    Plugins
                    <span class="nav-link-toggle"></span>
                  </a>
                  <ul class="nav nav-pills collapse" id="menu-plugins">
                    <li class="nav-item">
                      <a href="../docs/autosize.html" class="nav-link">
                        Autosize
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/input-mask.html" class="nav-link">
                        Form input mask
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/flags.html" class="nav-link">
                        Flags
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/payments.html" class="nav-link">
                        Payments
                      </a>
                    </li>
                    <li class="nav-item">
                      <a href="../docs/charts.html" class="nav-link">
                        Charts
                      </a>
                    </li>
                  </ul>
                </li>
                <li class="nav-item">
                  <a href="../changelog.html" class="nav-link">
                    <span class="nav-link-icon"><svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><circle cx="7" cy="18" r="2" /><circle cx="7" cy="6" r="2" /><circle cx="17" cy="6" r="2" /><line x1="7" y1="8" x2="7" y2="16" /><path d="M9 18h6a2 2 0 0 0 2 -2v-5" /><polyline points="14 14 17 11 20 14" /></svg>
                    </span>
                    Changelog
                    <span class="badge bg-blue-lt ms-auto">1.0.0-alpha.22</span>
                  </a>
                </li>
              </ul>
            </div>
            <div class="col-lg-9">
              <div class="card card-lg">
                <div class="card-body">
                  <div class="markdown">
                    <div>
                      <div class="d-flex mb-4">
                        <h1 class="mt-0">Introduction</h1>
                      </div>
                    </div>
                    <h2 id="what-is-tabler">What is Tabler?</h2>
                    <p>Tabler is a UI kit that speeds up the development process and makes it easier than ever! Built on the latest version of Bootstrap, it helps you create templates based on fully customizable and ready-to-use UI components, which can be used by both simple websites and sophisticated systems. With basic knowledge of HTML and CSS, you’ll be able to create dashboards that are fully functional and beautifully designed!</p>
                    <h2 id="what-are-the-benefits">What are the benefits?</h2>
                    <p>Tabler is a perfect solution if you want to create an interface which is not only user-friendly but also fully reponsive. Thanks to the big choice of ready-made components, you can customize your design and adapt it to the needs of even the most demanding users. On top of that, Tabler is an open source solution, continuously developed and improved by the open source community.</p>
                    <p>To start using Tabler, first you need to set up the environment.</p>
                    <h2 id="set-up-the-environment">Set up the environment</h2>
                    <p>To use our build system and run our documentation locally, you’ll need a copy of Tabler’s source files. Follow the steps below:</p>
                    <ol>
                      <li><a href="https://nodejs.org/download/">Install Node.js</a>, which we use to manage our dependencies.</li>
                      <li>Navigate to the root <code class="language-plaintext highlighter-rouge">/tabler</code> directory and run <code class="language-plaintext highlighter-rouge">npm install</code> to install our local dependencies listed in <code class="language-plaintext highlighter-rouge">package.json</code>.</li>
                      <li><a href="https://ruby-lang.org/en/documentation/installation/">Install Ruby</a> - the recommended version is <a href="https://cache.ruby-lang.org/pub/ruby/2.5/ruby-2.5.5.tar.gz">2.5.5</a>.</li>
                      <li><a href="https://bundler.io">Install Bundler</a> with <code class="language-plaintext highlighter-rouge">gem install bundler</code> and, finally, run <code class="language-plaintext highlighter-rouge">bundle install</code>. It will install all Ruby dependencies, such as <a href="https://jekyllrb.com">Jekyll and plugins</a>.</li>
                    </ol>
                    <h3 id="windows-users">Windows users</h3>
                    <ol>
                      <li><a href="https://git-scm.com/download/win">Install Git</a> in <code class="language-plaintext highlighter-rouge">C:\Program Files\git\bin</code> directory and run <code class="language-plaintext highlighter-rouge">npm config set script-shell "C:\Program Files\git\bin\bash.exe"</code> to change the default shell.</li>
                      <li><a href="https://rubyinstaller.org/downloads/">Install Ruby+Devkit</a> - recommended version is <a href="https://github.com/oneclick/rubyinstaller2/releases/download/RubyInstaller-2.5.5-1/rubyinstaller-devkit-2.5.5-1-x86.exe">2.5.5</a>.</li>
                      <li><a href="https://jekyllrb.com/docs/installation/windows/">Read guide</a> to get Jekyll up and running without problems.</li>
                    </ol>
                    <p>Once you’ve completed the setup, you’ll be able to run the various commands provided from the command line.</p>
                    <h2 id="build-tabler-locally">Build Tabler locally</h2>
                    <ol>
                      <li>From the root <code class="language-plaintext highlighter-rouge">/tabler</code> directory, run <code class="language-plaintext highlighter-rouge">npm run start</code> in the command line.</li>
                      <li>Open <a href="http://localhost:4000">http://localhost:4000</a> in your browser, and voilà.</li>
                      <li>Any change in <code class="language-plaintext highlighter-rouge">/pages</code> directory will build the application and refresh the page.</li>
                    </ol>
                    <h2 id="bugs-and-feature-requests">Bugs and feature requests</h2>
                    <p>Found a bug or have a feature request? <a href="https://github.com/tabler/tabler/issues/new">Please open a new issue</a>.</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
  
        <footer class="footer footer-transparent d-print-none">
          <div class="container">
            <div class="row text-center align-items-center flex-row-reverse">
              <div class="col-lg-auto ms-lg-auto">
                <ul class="list-inline list-inline-dots mb-0">
                  <li class="list-inline-item"><a href="../docs/index.html" class="link-secondary">Documentation</a></li>
                  <li class="list-inline-item"><a href="../license.html" class="link-secondary">License</a></li>
                  <li class="list-inline-item"><a href="https://github.com/tabler/tabler" target="_blank" class="link-secondary" rel="noopener">Source code</a></li>
                </ul>
              </div>
              <div class="col-12 col-lg-auto mt-3 mt-lg-0">
                <ul class="list-inline list-inline-dots mb-0">
                  <li class="list-inline-item">
                    Copyright &copy; 2021
                    <a href=".." class="link-secondary">Tabler</a>.
                    All rights reserved.
                  </li>
                  <li class="list-inline-item">
                    <a href="../changelog.html" class="link-secondary" rel="noopener">v1.0.0-alpha.22</a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </footer>
  
</template>


<!-- <script>
import './modal.scss'
import Title from '../Title/Title.vue';
// import './modal.js'

    export default {
    name: "modal",
    methods: {
        close() {
            this.$emit("close");
        },
    },
    components: { Title }
};
  </script>
  <template>
    <transition name="modal-fade">
      <div class="modal-backdrop">
        <div class="modal"
          role="dialog"
          aria-labelledby="modalTitle"
          aria-describedby="modalDescription"
        >
          <header
            class="modal-header"
            id="modalTitle"
          >
            <slot name="header">
              <Title title="Кошик" />
  
              <button
                type="button"
                class="btn-close"
                @click="close"
                aria-label="Close modal"
              >
                x
              </button>
            </slot>
          </header>
          <section
            class="modal-body"
            id="modalDescription"
          >
            <slot name="body">
              I'm the default body!
            </slot>
          </section>
          <footer class="modal-footer">
            <slot name="footer">
              I'm the default footer!
  
              <button
                type="button"
                class="btn-green"
                @click="close"
                aria-label="Close modal"
              >
                Close me!
              </button>
            </slot>
          </footer>
        </div>
      </div>
    </transition>
  </template>
  <style>
  
    .modal-header,
    .modal-footer {
      padding: 15px;
      display: flex;
    }
  
    .modal-header {
      border-bottom: 1px solid #eeeeee;
    }
  
    .modal-footer {
      border-top: 1px solid #eeeeee;
      justify-content: flex-end;
    }
  
    .modal-body {
      position: relative;
      padding: 20px 10px;
    }
  
    .btn-green {
      color: white;
      background: #4AAE9B;
      border: 1px solid #4AAE9B;
      border-radius: 2px;
    }
  </style> -->
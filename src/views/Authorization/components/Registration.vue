<template>
    <div class="registration">
        <div class="registration__inner">
            <div class="registration__item registration__left"></div>
            <div class="registration__item registration__right">
                <div class="registration__header">
                    <h3 class="registration__title">Create Account</h3>
                </div>
                <div class="registration__form">
                    <el-form
                        :label-position="'top'"
                    >
                    <el-row :gutter="14">
                        <el-col :span="10">
                            <el-form-item 
                                label="Name"
                                class="login__input"
                            >
                                <el-input 
                                    size="large"
                                    placeholder="John" 
                                />
                            </el-form-item>
                        </el-col>
                        <el-col :span="10">
                            <el-form-item 
                                label="Surname"
                                class="login__input"
                                >
                                    <el-input 
                                        size="large" 
                                        placeholder="Johnson" 
                                    />
                                </el-form-item>
                        </el-col>
                    </el-row>
                    <el-row>
                        <el-col :span="20">
                        <el-form-item label="E-mail"
                            class="login__input"
                        >
                            <el-input size="large" 
                                placeholder="example@stu.sdu.edu.kz" 
                            />
                        </el-form-item>
                        </el-col>
                    </el-row>
                    <el-row :gutter="14">
                        <el-col :span="10">
                            <el-form-item 
                                label="Status"
                                class="registration__input"
                            >
                            <el-select v-model="value" class="m-2" placeholder="ex: Student" size="large">
                                <el-option
                                    v-for="status in statuses"
                                    :key="status.id"
                                    :label="status.name"
                                    :value="status.id"
                                >
                                </el-option>
                            </el-select>
                            </el-form-item>
                        </el-col>
                        <el-col :span="10">
                            <el-form-item 
                                label="Education"
                                class="registration__input"
                            >
                            <el-select v-model="value" class="m-2" placeholder="ex: Bachelor" size="large">
                                <el-option
                                    v-for="edu in education"
                                    :key="edu.id"
                                    :label="edu.name"
                                    :value="edu.id"
                                >
                                </el-option>
                            </el-select>
                            </el-form-item>
                        </el-col>
                    </el-row>
                    <el-row>
                        <el-col :span="20">
                            <el-form-item label="Password"
                                class="login__input"
                            >
                                <el-input size="large" 
                                    placeholder="6+ Character, 1 Capital letter" 
                                />
                            </el-form-item>
                        </el-col>
                    </el-row>
                    <el-row>
                        <el-col :span="20">
                            <el-form-item>
                                <el-button type="primary" class="registration__btn">Sign Up</el-button>
                            </el-form-item>
                        </el-col>
                    </el-row>
                    </el-form>
                </div>                
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {
            user: {
                first_name: '',
                last_name: '',
                email: '',
                education: '',
                status: '',
                password: ''
            },
            statuses: [
                {
                    id: 1,
                    name: 'Student'
                },
                {
                    id: 2,
                    name: 'Supervisor'
                },
                {
                    id: 3,
                    name: 'Supervisor + Student'
                },
            ],
            education: [
                {
                    id: 1,
                    name: 'Bachelor'
                },
                {
                    id: 2,
                    name: 'Master'
                },
                {
                    id: 3,
                    name: 'Ph.D'
                },
            ]

        }
    }

}
</script>

<style lang="scss" scoped>
.registration {
    width: 100%;
    height: 100%;
    &__inner{
        display: flex;
        height: 100%;
    }
    &__left{
        width: 40%;
        background-color: #FAFBFC;
    }
    &__right{
        width: 60%;
        padding: 0 10px;
    }
    &__title{
        font-size: 30px;
        font-weight: 600;
    }
    &__btn{
        width: 100%;
        padding: 20px 0;
        font-size: 18px;
    }
}
</style>
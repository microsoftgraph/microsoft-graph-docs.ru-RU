---
title: Связывание учетной записи Office 365 с Azure AD для создания приложений и управления ими
description: 'Для проверки подлинности приложений с помощью Microsoft Azure Active Directory необходимо зарегистрировать их в Azure AD. Именно здесь хранятся сведения об учетной записи пользователя Office 365 и приложениях. Чтобы управлять Azure Active Directory на портале Azure, необходима подписка на Microsoft Azure. Управлять пользователями, ролями и приложениями можно с помощью портала в Microsoft Azure. '
localization_priority: Normal
ms.openlocfilehash: cf369f1f289c435cbd488d4c51e558d75a5e080e
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969782"
---
# <a name="associate-your-office-365-account-with-azure-ad-to-create-and-manage-apps"></a><span data-ttu-id="1f568-106">Связывание учетной записи Office 365 с Azure AD для создания приложений и управления ими</span><span class="sxs-lookup"><span data-stu-id="1f568-106">Associate your Office 365 account with Azure AD to create and manage apps</span></span>

<span data-ttu-id="1f568-107">Для проверки подлинности приложений с помощью Microsoft Azure Active Directory необходимо зарегистрировать их в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1f568-107">To authenticate your applications using Microsoft Azure Active Directory (Azure AD), you need to register them in Azure AD.</span></span> <span data-ttu-id="1f568-108">Именно здесь хранятся сведения об учетной записи пользователя Office 365 и приложениях.</span><span class="sxs-lookup"><span data-stu-id="1f568-108">This is where Office 365 user account and application information is stored.</span></span> <span data-ttu-id="1f568-109">Чтобы управлять Azure Active Directory на портале Azure, необходима подписка на Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="1f568-109">To manage Azure AD through the Azure portal, you need a Microsoft Azure subscription.</span></span> <span data-ttu-id="1f568-110">Управлять пользователями, ролями и приложениями можно с помощью портала в Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="1f568-110">You can use the portal in Microsoft Azure to manage users, roles, and apps.</span></span>

<span data-ttu-id="1f568-111">В этой статье показано, как связать учетную запись Office 365 с Azure Active Directory для создания приложений и управления ими.</span><span class="sxs-lookup"><span data-stu-id="1f568-111">This article shows you how to associate your Office 365 account with Azure AD to create and manage apps.</span></span>

 ><span data-ttu-id="1f568-p103">**Примечание.** В этой статье в качестве поставщика проверки подлинности для приложения используется Azure AD. Если вы используете конечную точку Azure AD версии 2.0, выполнять это действие не требуется. Дополнительные сведения см. в статье [Проверка подлинности в приложении с помощью Microsoft Graph](/graph/auth).</span><span class="sxs-lookup"><span data-stu-id="1f568-p103">**Note:** This article uses Azure AD as the authentication provider for your app. If you're using the Azure AD v2.0 endpoint, you don't need to perform this step. For more information, see [App authentication with Microsoft Graph](/graph/auth).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f568-115">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f568-115">Prerequisites</span></span>

<span data-ttu-id="1f568-116">**Учетная запись Office 365 для бизнеса**.</span><span class="sxs-lookup"><span data-stu-id="1f568-116">**Office 365 for business account**</span></span>

<span data-ttu-id="1f568-117">Если у вас нет учетной записи Office 365 для бизнеса, вы можете:</span><span class="sxs-lookup"><span data-stu-id="1f568-117">If you don't have an existing Office 365 for business account, you can:</span></span>

- <span data-ttu-id="1f568-118">Регистрация в [плане Office 365 для бизнеса](https://products.office.com/business/compare-office-365-for-business-plans)</span><span class="sxs-lookup"><span data-stu-id="1f568-118">Sign up for an [Office 365 for business plan](https://products.office.com/business/compare-office-365-for-business-plans)</span></span> 
- <span data-ttu-id="1f568-119">[Присоединяйтесь к программе для разработчиков office 365](https://aka.ms/devprogramsignup) и получите бесплатную подписку на Office 365 с помощью одного года.</span><span class="sxs-lookup"><span data-stu-id="1f568-119">[Join the Office 365 Developer Program](https://aka.ms/devprogramsignup) and get a free one-year subscription to Office 365.</span></span>

<span data-ttu-id="1f568-120">**Подписка на Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="1f568-120">**Microsoft Azure subscription**</span></span>

- <span data-ttu-id="1f568-121">Если у вас есть подписка на Microsoft Azure, вы можете связать с ней свою подписку на Office 365 для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f568-121">If you can have an existing Microsoft Azure subscription, you can associate your Office 365 for business subscription with it.</span></span>

- <span data-ttu-id="1f568-122">В противном случае вам понадобится создать подписку на Azure и связать ее с учетной записью Office 365, чтобы регистрировать приложения и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="1f568-122">Otherwise, you'll need to create a new Azure subscription and associate it with your Office 365 account in order to register and manage apps.</span></span>


<!---<a name="bk_AssociateExistingAzureSubscription"> </a>-->

## <a name="to-associate-an-existing-azure-subscription-with-your-office-365-account"></a><span data-ttu-id="1f568-123">Связывание подписки на Azure с учетной записью Office 365</span><span class="sxs-lookup"><span data-stu-id="1f568-123">To associate an existing Azure subscription with your Office 365 account</span></span>


1. <span data-ttu-id="1f568-124">Войдите на [портал Microsoft Azure](https://portal.azure.com), используя свои учетные данные Azure (например, идентификатор Майкрософт, такой как polzovatel@live.com).</span><span class="sxs-lookup"><span data-stu-id="1f568-124">Log on to the  [Microsoft Azure portal](https://portal.azure.com) with your existing Azure credentials (for example, your Microsoft ID such as user@live.com).</span></span>

2. <span data-ttu-id="1f568-125">Выберите узел **Active Directory**, откройте вкладку **Каталог**, а затем в нижней части экрана выберите элемент **Создать**.</span><span class="sxs-lookup"><span data-stu-id="1f568-125">Select the  **Active Directory** node, then select the **Directory** tab and, at the bottom of the screen, select **New**.</span></span>

4. <span data-ttu-id="1f568-126">В меню **Создать** выберите пункты **Active Directory** > **Каталог** > **Настраиваемое создание**.</span><span class="sxs-lookup"><span data-stu-id="1f568-126">On the **New** menu, select **Active Directory** > **Directory** > **Custom Create**.</span></span>

5. <span data-ttu-id="1f568-p104">В раскрывающемся списке **Каталог** раздела **Добавление каталога** выберите пункт **Использовать существующий каталог**. Установите флажок **Я готов к выходу из системы**, а затем установите еще один флажок в правом нижнем углу.</span><span class="sxs-lookup"><span data-stu-id="1f568-p104">In **Add directory**, in the **Directory** dropdown box, select  **Use existing directory**. Check **I am ready to be signed out**, and then select the check mark in the lower-right corner.</span></span>

    <span data-ttu-id="1f568-129">Вы вернетесь на портал Azure.</span><span class="sxs-lookup"><span data-stu-id="1f568-129">This brings you back to the Azure portal.</span></span>

3. <span data-ttu-id="1f568-130">Войдите, используя сведения учетной записи Office 365.</span><span class="sxs-lookup"><span data-stu-id="1f568-130">Log in with your Office 365 account information.</span></span>

    <span data-ttu-id="1f568-131">Вам будет предложено использовать каталог с Azure.</span><span class="sxs-lookup"><span data-stu-id="1f568-131">You will be prompted whether to use your directory with Azure.</span></span>

    ><span data-ttu-id="1f568-132">**Важно!** Чтобы связать свою учетную запись Office 365 с Azure AD, вам понадобится учетная запись Office 365 бизнес с правами глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="1f568-132">**Important:** To associate your Office 365 account with Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span>


4. <span data-ttu-id="1f568-133">Последовательно выберите элементы **Продолжить** и **Выйти**.</span><span class="sxs-lookup"><span data-stu-id="1f568-133">Select  **continue**, and then **Sign out now**.</span></span>

5. <span data-ttu-id="1f568-p105">Закройте браузер и снова откройте [портал](https://manage.windowsazure.com). В противном случае появится сообщение об отказе в доступе.</span><span class="sxs-lookup"><span data-stu-id="1f568-p105">Close the browser and reopen the  [portal](https://manage.windowsazure.com). Otherwise, you will get an access denied error.</span></span>


6. <span data-ttu-id="1f568-p106">Снова войдите, используя свои учетные данные Azure (например, идентификатор Майкрософт, такой как polzovatel@live.com). Перейдите к узлу **Active Directory**. Учетная запись Office 365 должна появиться в разделе **Каталог**.</span><span class="sxs-lookup"><span data-stu-id="1f568-p106">Log on again with your existing Azure credentials (for example, your Microsoft ID such as user@live.com). Go to the  **Active Directory** node and, under **Directory**, you should now see your Office 365 account listed.</span></span>


<!--<a name="bk_AssociateNewAzureSubscription"> </a>-->

## <a name="to-create-a-new-azure-subscription-and-associate-it-with-your-office-365-account"></a><span data-ttu-id="1f568-138">Создание подписки на Azure и ее связывание с учетной записью Office 365</span><span class="sxs-lookup"><span data-stu-id="1f568-138">To create a new Azure subscription and associate it with your Office 365 account</span></span>


1. <span data-ttu-id="1f568-p107">Войдите в Office 365. На **главной** странице выберите значок **Администратор**, чтобы открыть Центр администрирования Office 365.</span><span class="sxs-lookup"><span data-stu-id="1f568-p107">Log on to Office 365. From the **Home** page, select the **Admin** icon to open the Office 365 admin center.</span></span>
2. <span data-ttu-id="1f568-141">На странице меню в левой части страницы найдите раздел **Администратор** и выберите пункт **Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="1f568-141">In the menu page along the left side of the page, scroll down to **Admin** and select **Azure AD**.</span></span>

    ><span data-ttu-id="1f568-142">**Важно!** Чтобы открыть Центр администрирования Office 365 и получить доступ к Azure AD, вам понадобится учетная запись Office 365 бизнес с правами глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="1f568-142">**Important:** To open the Office 365 admin center, and access Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span>

3. <span data-ttu-id="1f568-143">Создайте подписку.</span><span class="sxs-lookup"><span data-stu-id="1f568-143">Create a new subscription.</span></span>

    <span data-ttu-id="1f568-p108">Если вы используете пробную версию Office 365, отобразится сообщение о том, что служба Azure AD доступна только пользователям с платной подпиской. Вы все равно можете создать бесплатную 30-дневную пробную подписку на Azure, но для этого необходимо выполнить несколько дополнительных действий:</span><span class="sxs-lookup"><span data-stu-id="1f568-p108">If you're using a trial version of Office 365, you'll see a message telling you that Azure AD is limited to customers with paid services. You can still create a trial 30-day Azure subscription at no charge, but you'll need to perform a few extra steps:</span></span>

    1. <span data-ttu-id="1f568-146">Выберите свою страну или регион, а затем выберите элемент **Подписка Azure**.</span><span class="sxs-lookup"><span data-stu-id="1f568-146">Select your country or region, and then choose **Azure subscription**.</span></span>
    2. <span data-ttu-id="1f568-p109">Введите свои личные сведения. Введите свой контактный номер телефона и укажите предпочитаемый способ проверки (с помощью SMS или звонка).</span><span class="sxs-lookup"><span data-stu-id="1f568-p109">Enter your personal information. For verification purposes, enter a telephone number at which you can be reached, and specify whether you want to be sent a text message or called.</span></span>
    3. <span data-ttu-id="1f568-149">Получив код подтверждения, введите его и нажмите **Проверить код**.</span><span class="sxs-lookup"><span data-stu-id="1f568-149">When you receive your verification code, enter it and choose **Verify code**.</span></span>
    4. <span data-ttu-id="1f568-150">Введите сведения об оплате, просмотрите соглашение и выберите пункт **Регистрация**.</span><span class="sxs-lookup"><span data-stu-id="1f568-150">Enter payment information, check the agreement, and select **Sign up**.</span></span>

        <span data-ttu-id="1f568-151">Никакие средства с вашей кредитной карты списаны не будут.</span><span class="sxs-lookup"><span data-stu-id="1f568-151">Your credit card will not be charged.</span></span>

        <span data-ttu-id="1f568-152">Не закрывайте и не обновляйте браузер во время создания подписки на Azure.</span><span class="sxs-lookup"><span data-stu-id="1f568-152">Do not close or refresh your browser while your Azure subscription is being created.</span></span>

4. <span data-ttu-id="1f568-153">После создания подписки на Azure выберите элемент **Портал**.</span><span class="sxs-lookup"><span data-stu-id="1f568-153">When your Azure subscription is created, choose  **Portal**.</span></span>

5. <span data-ttu-id="1f568-p110">Откроется обзор Azure. Вы можете просмотреть его или нажать кнопку **X**, чтобы закрыть окно.</span><span class="sxs-lookup"><span data-stu-id="1f568-p110">The Azure Tour appears. You can view it, or choose  **X** to close it.</span></span>

    <span data-ttu-id="1f568-p111">Теперь в подписке на Azure должны появиться все элементы. Вы увидите каталог с именем вашего клиента Office 365.</span><span class="sxs-lookup"><span data-stu-id="1f568-p111">You should now see all items in your Azure subscription. It lists a directory with the name of your Office 365 tenant.</span></span>

## <a name="see-also"></a><span data-ttu-id="1f568-158">См. также</span><span class="sxs-lookup"><span data-stu-id="1f568-158">See also</span></span>
- [<span data-ttu-id="1f568-159">Основные сведения о регистрации приложения в Azure AD</span><span class="sxs-lookup"><span data-stu-id="1f568-159">Basics of Registering an Application in Azure AD</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)
- [<span data-ttu-id="1f568-160">Интеграция приложений с Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1f568-160">Add, update, or remove an application in Azure AD</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-integrating-applications/)

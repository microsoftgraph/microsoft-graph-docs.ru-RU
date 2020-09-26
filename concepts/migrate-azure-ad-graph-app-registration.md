---
title: Рассмотрение проблем с регистрацией приложений, разрешениями и согласия миграции
description: Описание регистрации приложений, разрешений и миграции согласия из Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 8cca43199d8549841087a84d1bd275e38f09efdb
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288345"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="1a5e7-103">Проверка регистрации приложения, разрешений и согласия</span><span class="sxs-lookup"><span data-stu-id="1a5e7-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="1a5e7-104">Эта статья входит в *Шаг 3: Ознакомьтесь со сведениями о* [процессе миграции приложений](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e7-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="1a5e7-105">Для любого обновления приложения необходимо учитывать три области.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="1a5e7-106">**Регистрация приложений**: вы можете продолжать использовать существующую регистрацию приложения ( `appId` ) в коде приложения.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="1a5e7-107">**Нет необходимости** повторно регистрировать приложение для миграции в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="1a5e7-108">Просто обновите код, протестируйте его в значительной степени, а затем разверните обновление.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="1a5e7-109">**Разрешения**: вы можете продолжать использовать существующие настроенные разрешения для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-109">**Permissions**: You can continue to use the existing configured permissions for your app.</span></span> <span data-ttu-id="1a5e7-110">Вам не нужно запрашивать новые разрешения, так как разрешения Azure AD Graph совместно используются в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-110">You do not have to request new permissions because Azure AD Graph permissions are shared with Microsoft Graph.</span></span>

    <span data-ttu-id="1a5e7-111">Например, если у имеющегося приложения есть разрешение _User. Read. ALL_ и _Group. Read. ALL_ , эти разрешения также неявно предоставляются обновленному приложению для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-111">For example, if your existing app has _User.Read.All_ and _Group.Read.All_ permissions, those permissions are implicitly granted to your updated app for Microsoft Graph as well.</span></span>

    <span data-ttu-id="1a5e7-112">Если ваше обновление также инкудес использовать функции или возможности, недоступные для Azure AD Graph, вам, скорее всего, потребуется запросить разрешения для этих новых функций.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="1a5e7-113">В этом случае вы можете переключить приложение для использования MSAL и конечной точки v2, а также динамически запрашивать дополнительное/добавочное согласие.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="1a5e7-114">Дополнительные сведения о переходе на MSAL в окне [пересмотр библиотеки проверки подлинности приложений](./migrate-azure-ad-graph-authentication-library.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e7-114">Find more details about switching to MSAL in [review app authentication library changes](./migrate-azure-ad-graph-authentication-library.md).</span></span>

- <span data-ttu-id="1a5e7-115">**Согласие**: конечные пользователи могут продолжать использовать ваше приложение без запроса на предоставление разрешения.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-115">**Consent**: End-users can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="1a5e7-116">Пользователи, которые уже предоставили согласие на доступ к своим данным, могут продолжать использовать ваше приложение после обновления до использования Microsoft Graph без запроса подтверждения.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span>

<span data-ttu-id="1a5e7-117">В таких областях не должно возникнуть проблем с простыми проектами миграции.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-117">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="1a5e7-118">Тем не менее, если вы используете новые функции, службы или добавляете дополнительные возможности, могут потребоваться новые разрешения и разрешение конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-118">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="1a5e7-119">В таких случаях разрешение запрашивается при обновлении маркеров.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-119">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1a5e7-120">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1a5e7-120">Next Steps</span></span>

- <span data-ttu-id="1a5e7-121">Сведения о различиях между [библиотеками проверки подлинности](migrate-azure-ad-graph-authentication-library.md) в Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5e7-121">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="1a5e7-122">Снова просмотрите [Контрольный список](migrate-azure-ad-graph-planning-checklist.md) .</span><span class="sxs-lookup"><span data-stu-id="1a5e7-122">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>
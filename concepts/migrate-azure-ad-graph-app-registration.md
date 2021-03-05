---
title: Просмотр вопросов регистрации, разрешений и миграции согласия
description: Описывает миграцию регистрации, разрешений и согласия приложений из Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 06eeb5adeb1625559ca838a04590d2db65a03f97
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470650"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="02a5e-103">Просмотр регистрации, разрешений и согласия приложений</span><span class="sxs-lookup"><span data-stu-id="02a5e-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="02a5e-104">Эта статья является *частью шага 3: просмотрите* сведения о процессе переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="02a5e-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="02a5e-105">Для любого обновления приложения необходимо учитывать три области:</span><span class="sxs-lookup"><span data-stu-id="02a5e-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="02a5e-106">**Регистрация приложений.** Вы можете продолжать использовать существующую регистрацию приложений `appId` () в коде приложения.</span><span class="sxs-lookup"><span data-stu-id="02a5e-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="02a5e-107">Чтобы **перейти** в Microsoft Graph, не нужно перерегистрировать приложение.</span><span class="sxs-lookup"><span data-stu-id="02a5e-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="02a5e-108">Просто обновите код, протестировать и развернуть обновление.</span><span class="sxs-lookup"><span data-stu-id="02a5e-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="02a5e-109">**Разрешения.** Необходимо изменить настроенные разрешения на эквивалентные разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02a5e-109">**Permissions**: You should change your configured permissions to the equivalent Microsoft Graph permissions.</span></span> <span data-ttu-id="02a5e-110">Делегированная лицензия, выданная для Azure AD Graph, будет неявно считаться предоставленной и для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02a5e-110">Delegated permissions which were granted for Azure AD Graph will be implicitly considered granted for Microsoft Graph also.</span></span> <span data-ttu-id="02a5e-111">Разрешения приложения (роли приложений) должны быть снова предоставлены.</span><span class="sxs-lookup"><span data-stu-id="02a5e-111">Application permissions (app roles) will need to be granted again.</span></span>

    <span data-ttu-id="02a5e-112">Если обновление также не позволяет использовать функции или возможности, недоступные Azure AD Graph, вам, скорее всего, потребуется запрашивать разрешения для этих новых функций.</span><span class="sxs-lookup"><span data-stu-id="02a5e-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="02a5e-113">В этом случае можно переключить приложение на использование MSAL и конечной точки v2 и динамически запрашивать дополнительное/дополнительное согласие.</span><span class="sxs-lookup"><span data-stu-id="02a5e-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="02a5e-114">Дополнительные сведения о переходе на MSAL можно найти в обзоре изменений библиотеки [проверки подлинности приложений.](./migrate-azure-ad-graph-authentication-library.md)</span><span class="sxs-lookup"><span data-stu-id="02a5e-114">Find more details about switching to MSAL in [review app authentication library changes](./migrate-azure-ad-graph-authentication-library.md).</span></span>

- <span data-ttu-id="02a5e-115">**Согласие.** Конечные пользователи, которые уже предоставили согласие на делегирование разрешений (или для которых согласие уже было предоставлено администратором), могут продолжать использовать ваше приложение без повторного запроса на предоставление согласия.</span><span class="sxs-lookup"><span data-stu-id="02a5e-115">**Consent**: End-users who have already granted consent for delegated permissions (or for whom consent has already been granted by an admin) can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="02a5e-116">Пользователи, которые уже дали согласие вашему приложению на доступ к своим данным, могут продолжать использовать ваше приложение после обновления, чтобы использовать Microsoft Graph, не получив повторного согласия.</span><span class="sxs-lookup"><span data-stu-id="02a5e-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span> <span data-ttu-id="02a5e-117">Для получения согласия будут предложены новые пользователи.</span><span class="sxs-lookup"><span data-stu-id="02a5e-117">New users will be prompted for consent.</span></span>

<span data-ttu-id="02a5e-118">Простые проекты миграции не должны испытывать проблем в этих областях.</span><span class="sxs-lookup"><span data-stu-id="02a5e-118">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="02a5e-119">Однако, если вы используете новые функции, службы или добавляете дополнительные возможности, возможно, потребуются новые разрешения и согласие конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="02a5e-119">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="02a5e-120">В таких случаях при обновлении маркеров запрашивается согласие.</span><span class="sxs-lookup"><span data-stu-id="02a5e-120">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="02a5e-121">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="02a5e-121">Next Steps</span></span>

- <span data-ttu-id="02a5e-122">Узнайте [о различиях](migrate-azure-ad-graph-authentication-library.md) в библиотеке проверки подлинности между Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02a5e-122">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="02a5e-123">Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.</span><span class="sxs-lookup"><span data-stu-id="02a5e-123">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>

---
title: Использование REST API для OneNote
description: 'Microsoft Graph позволяет вашему приложению получать авторизованный доступ к записным книжкам, разделам и страницам OneNote в личной или организационной учетной записи. Имея соответствующие разрешения приложения или делегированные разрешения, приложение может получать доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: 0c13ebeb6381e894684a14be42772d69b5d31e62
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630328"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="dcda6-104">Использование REST API для OneNote</span><span class="sxs-lookup"><span data-stu-id="dcda6-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcda6-105">Microsoft Graph позволяет вашему приложению получать авторизованный доступ к записным книжкам, разделам и страницам OneNote в личной или организационной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="dcda6-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="dcda6-106">Имея [соответствующие разрешения приложения или делегированные разрешения](/graph/permissions-reference#notes-permissions), приложение может получать доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="dcda6-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="dcda6-107">Корневой URL-адрес</span><span class="sxs-lookup"><span data-stu-id="dcda6-107">Root URL</span></span>
<span data-ttu-id="dcda6-108">Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.</span><span class="sxs-lookup"><span data-stu-id="dcda6-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="dcda6-109">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="dcda6-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="dcda6-110">Значение `v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="dcda6-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="dcda6-111">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="dcda6-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="dcda6-112">Функции бета-версии конечной точки могут меняться. Не рекомендуем использовать ее в рабочем коде.</span><span class="sxs-lookup"><span data-stu-id="dcda6-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="dcda6-113">Местоположение может представлять собой записные книжки для пользователей в Microsoft 365 или OneDrive для пользователей, групповые записные книжки или записные книжки группы SharePoint, размещенные на сайте Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dcda6-113">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

![Стек разработки API OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

## <a name="user-notebooks"></a><span data-ttu-id="dcda6-115">Записные книжки пользователей</span><span class="sxs-lookup"><span data-stu-id="dcda6-115">User notebooks</span></span>
<span data-ttu-id="dcda6-116">Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="dcda6-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="dcda6-117">Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="dcda6-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="dcda6-118">Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="dcda6-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="dcda6-119">Используйте API для работы с [пользователями](users.md).</span><span class="sxs-lookup"><span data-stu-id="dcda6-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="dcda6-120">**Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="dcda6-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

## <a name="group-notebooks"></a><span data-ttu-id="dcda6-121">Записные книжки группы</span><span class="sxs-lookup"><span data-stu-id="dcda6-121">Group notebooks</span></span>

<span data-ttu-id="dcda6-122">Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="dcda6-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="sharepoint-site-notebooks"></a><span data-ttu-id="dcda6-123">Записные книжки на сайте SharePoint</span><span class="sxs-lookup"><span data-stu-id="dcda6-123">SharePoint site notebooks</span></span>
<span data-ttu-id="dcda6-124">Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="dcda6-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="whats-new"></a><span data-ttu-id="dcda6-125">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="dcda6-125">What's new</span></span>
<span data-ttu-id="dcda6-126">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="dcda6-126">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

---
title: Использование REST API для OneNote
description: 'Microsoft Graph позволяет приложению получать авторизованный доступ к записным книжкам OneNote, разделам и страницам пользователя в личной учетной записи или организации. Используя соответствующие разрешения делегирования или приложения, ваше приложение может получить доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566047"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="0529d-104">Использование REST API для OneNote</span><span class="sxs-lookup"><span data-stu-id="0529d-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0529d-105">Microsoft Graph позволяет приложению получать авторизованный доступ к записным книжкам OneNote, разделам и страницам пользователя в личной учетной записи или организации.</span><span class="sxs-lookup"><span data-stu-id="0529d-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="0529d-106">Используя [соответствующие разрешения делегирования или приложения](/graph/permissions-reference#notes-permissions), ваше приложение может получить доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0529d-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="0529d-107">Корневой URL-адрес</span><span class="sxs-lookup"><span data-stu-id="0529d-107">Root URL</span></span>
<span data-ttu-id="0529d-108">В корневом URL-АДРЕСе службы OneNote для всех вызовов API OneNote используется следующий формат.</span><span class="sxs-lookup"><span data-stu-id="0529d-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="0529d-109">`version` Сегмент в URL-адресе представляет версию Microsoft Graph, которую вы хотите использовать:</span><span class="sxs-lookup"><span data-stu-id="0529d-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="0529d-110">Значение `v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="0529d-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="0529d-111">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="0529d-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="0529d-112">Функции и функции в конечной точке бета-версии могут измениться; Мы не рекомендуем использовать его в рабочем коде.</span><span class="sxs-lookup"><span data-stu-id="0529d-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="0529d-113">Местоположение может представлять собой записные книжки для пользователей в Office 365 или OneDrive для пользователей, групповых записных книжек или размещенных на сайте SharePoint записных книжек группы в Office 365.</span><span class="sxs-lookup"><span data-stu-id="0529d-113">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Стек разработки API OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="0529d-115">Записные книжки пользователя</span><span class="sxs-lookup"><span data-stu-id="0529d-115">User notebooks</span></span>
<span data-ttu-id="0529d-116">Чтобы получить доступ к личным записным книжкам в OneDrive для бизнеса или OneDrive для бизнеса, используйте один из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="0529d-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="0529d-117">Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="0529d-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="0529d-118">Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="0529d-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="0529d-119">Использование API [пользователей](users.md) .</span><span class="sxs-lookup"><span data-stu-id="0529d-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="0529d-120">**Примечание:** Вы можете получить идентификаторы пользователей, выполнив запрос GET `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="0529d-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="0529d-121">Записные книжки для групп</span><span class="sxs-lookup"><span data-stu-id="0529d-121">Group notebooks</span></span>

<span data-ttu-id="0529d-122">Чтобы получить доступ к записным книжкам, принадлежащим группе, используйте следующий корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="0529d-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="0529d-123">Записные книжки сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="0529d-123">SharePoint site notebooks</span></span>
<span data-ttu-id="0529d-124">Чтобы получить доступ к записным книжкам, принадлежащим сайту группы SharePoint, используйте следующий корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="0529d-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

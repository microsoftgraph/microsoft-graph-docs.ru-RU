---
title: Использование REST API для OneNote
description: 'Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи. С соответствующими делегированной или разрешения приложения, приложение может получать доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525628"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="fbe07-104">Использование REST API для OneNote</span><span class="sxs-lookup"><span data-stu-id="fbe07-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbe07-105">Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи.</span><span class="sxs-lookup"><span data-stu-id="fbe07-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="fbe07-106">С [соответствующими разрешениями делегированные или приложения](/graph/permissions-reference#notes-permissions)приложение может доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="fbe07-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="fbe07-107">Корневой URL-адрес</span><span class="sxs-lookup"><span data-stu-id="fbe07-107">Root URL</span></span>
<span data-ttu-id="fbe07-108">Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.</span><span class="sxs-lookup"><span data-stu-id="fbe07-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="fbe07-109">`version` Сегмента в URL-адрес представляет версию Microsoft Graph, который вы хотите использовать:</span><span class="sxs-lookup"><span data-stu-id="fbe07-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="fbe07-110">Значение `v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="fbe07-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="fbe07-111">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="fbe07-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="fbe07-112">Возможности и функции в конечной точке бета-версии может изменяться; не рекомендуется использовать в рабочем коде.</span><span class="sxs-lookup"><span data-stu-id="fbe07-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="fbe07-113">В качестве расположений можно задавать записные книжки пользователя в Office 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Office 365.</span><span class="sxs-lookup"><span data-stu-id="fbe07-113">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Стек разработки API-интерфейса OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="fbe07-115">Записные книжки пользователя</span><span class="sxs-lookup"><span data-stu-id="fbe07-115">User notebooks</span></span>
<span data-ttu-id="fbe07-116">Для доступа к личные записные книжки на потребителей OneDrive или OneDrive для бизнеса, используйте один из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="fbe07-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="fbe07-117">Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="fbe07-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="fbe07-118">Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="fbe07-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="fbe07-119">С помощью API [пользователей](users.md) .</span><span class="sxs-lookup"><span data-stu-id="fbe07-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="fbe07-120">**Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="fbe07-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="fbe07-121">Группа записных книжек</span><span class="sxs-lookup"><span data-stu-id="fbe07-121">Group notebooks</span></span>

<span data-ttu-id="fbe07-122">Для доступа к записные книжки, владельцем которых является группу, используйте следующие корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="fbe07-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="fbe07-123">Записные книжки сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="fbe07-123">SharePoint site notebooks</span></span>
<span data-ttu-id="fbe07-124">Для доступа к портативные компьютеры, принадлежащие сайту группы SharePoint, используйте следующие корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="fbe07-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

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

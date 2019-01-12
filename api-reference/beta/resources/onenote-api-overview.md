---
title: Использование REST API для OneNote
description: 'Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи. С соответствующими делегированной или разрешения приложения, приложение может получать доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ff17f7fbe5f15752bc272b79f3f741180f8d6417
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953002"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="e1d0b-104">Использование REST API для OneNote</span><span class="sxs-lookup"><span data-stu-id="e1d0b-104">Use the OneNote REST API</span></span>

> <span data-ttu-id="e1d0b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1d0b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1d0b-107">Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-107">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="e1d0b-108">С [соответствующими разрешениями делегированные или приложения](/graph/permissions-reference#notes-permissions)приложение может доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-108">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="e1d0b-109">Корневой URL-адрес</span><span class="sxs-lookup"><span data-stu-id="e1d0b-109">Root URL</span></span>
<span data-ttu-id="e1d0b-110">Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-110">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="e1d0b-111">`version` Сегмента в URL-адрес представляет версию Microsoft Graph, который вы хотите использовать:</span><span class="sxs-lookup"><span data-stu-id="e1d0b-111">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="e1d0b-112">Значение `v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-112">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="e1d0b-113">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-113">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="e1d0b-114">Возможности и функции в конечной точке бета-версии может изменяться; не рекомендуется использовать в рабочем коде.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-114">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="e1d0b-115">Расположение может быть записных книжек пользователя на Office 365 или потребитель OneDrive, группа записных книжек или записных книжек размещенного сайта группы SharePoint на Office 365.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-115">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Стек разработки API-интерфейса OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="e1d0b-117">Записные книжки пользователя</span><span class="sxs-lookup"><span data-stu-id="e1d0b-117">User notebooks</span></span>
<span data-ttu-id="e1d0b-118">Для доступа к личные записные книжки на потребителей OneDrive или OneDrive для бизнеса, используйте один из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="e1d0b-118">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="e1d0b-119">Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="e1d0b-119">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="e1d0b-120">Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-120">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="e1d0b-121">С помощью API [пользователей](users.md) .</span><span class="sxs-lookup"><span data-stu-id="e1d0b-121">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="e1d0b-122">**Примечание:** Идентификаторы пользователей можно получить, выбрав запрос GET на `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="e1d0b-122">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="e1d0b-123">Группа записных книжек</span><span class="sxs-lookup"><span data-stu-id="e1d0b-123">Group notebooks</span></span>

<span data-ttu-id="e1d0b-124">Для доступа к записные книжки, владельцем которых является группу, используйте следующие корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="e1d0b-124">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="e1d0b-125">Записные книжки сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="e1d0b-125">SharePoint site notebooks</span></span>
<span data-ttu-id="e1d0b-126">Для доступа к портативные компьютеры, принадлежащие сайту группы SharePoint, используйте следующие корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="e1d0b-126">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

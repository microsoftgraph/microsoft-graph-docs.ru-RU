---
title: Тип ресурса publicClient
description: Задает параметры для без веб-приложения или веб-Api. (например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)
localization_priority: Normal
ms.openlocfilehash: c466c91f90ac8adc2bf3806fa212e0b01e6d2507
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864199"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="f09de-104">Тип ресурса publicClient</span><span class="sxs-lookup"><span data-stu-id="f09de-104">publicClient resource type</span></span>

> <span data-ttu-id="f09de-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f09de-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f09de-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f09de-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f09de-107">Задает параметры для без веб-приложения или веб-Api.</span><span class="sxs-lookup"><span data-stu-id="f09de-107">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="f09de-108">(например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)</span><span class="sxs-lookup"><span data-stu-id="f09de-108">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="f09de-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f09de-109">Properties</span></span>

| <span data-ttu-id="f09de-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f09de-110">Property</span></span> | <span data-ttu-id="f09de-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f09de-111">Type</span></span> | <span data-ttu-id="f09de-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f09de-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f09de-113">redirectUris</span><span class="sxs-lookup"><span data-stu-id="f09de-113">redirectUris</span></span>|<span data-ttu-id="f09de-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f09de-114">String collection</span></span>| <span data-ttu-id="f09de-115">Указывает URL-адресов, которые будут отправлены маркеры пользователя для входа в или отправки коды авторизации коды URI, OAuth 2.0 и маркеры доступа для перенаправления.</span><span class="sxs-lookup"><span data-stu-id="f09de-115">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f09de-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f09de-116">JSON representation</span></span>
<span data-ttu-id="f09de-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f09de-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра объекта, например сообщения получателю и календарь владельцем.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c06849a73f4246653b8d78dcd392c4e4f6686a46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932793"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="6e286-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="6e286-103">emailAddress resource type</span></span>

> <span data-ttu-id="6e286-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e286-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e286-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e286-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e286-106">Представляет имя и SMTP-адрес экземпляра объекта, например сообщения получателю и календарь владельцем.</span><span class="sxs-lookup"><span data-stu-id="6e286-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="6e286-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e286-107">Properties</span></span>
| <span data-ttu-id="6e286-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e286-108">Property</span></span>     | <span data-ttu-id="6e286-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e286-109">Type</span></span>   |<span data-ttu-id="6e286-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e286-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e286-111">address</span><span class="sxs-lookup"><span data-stu-id="6e286-111">address</span></span>|<span data-ttu-id="6e286-112">String</span><span class="sxs-lookup"><span data-stu-id="6e286-112">String</span></span>|<span data-ttu-id="6e286-113">Адрес электронной почты экземпляр сущности.</span><span class="sxs-lookup"><span data-stu-id="6e286-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="6e286-114">name</span><span class="sxs-lookup"><span data-stu-id="6e286-114">name</span></span>|<span data-ttu-id="6e286-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6e286-115">String</span></span>|<span data-ttu-id="6e286-116">Отображаемое имя экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6e286-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e286-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e286-117">JSON representation</span></span>

<span data-ttu-id="6e286-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e286-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра объекта, например сообщения получателю и календарь владельцем.
localization_priority: Normal
ms.openlocfilehash: 5286334378aa5d208cf171ecab0bdc1777a4073b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871227"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="b7d16-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="b7d16-103">emailAddress resource type</span></span>

> <span data-ttu-id="b7d16-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7d16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7d16-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7d16-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7d16-106">Представляет имя и SMTP-адрес экземпляра объекта, например сообщения получателю и календарь владельцем.</span><span class="sxs-lookup"><span data-stu-id="b7d16-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="b7d16-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7d16-107">Properties</span></span>
| <span data-ttu-id="b7d16-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7d16-108">Property</span></span>     | <span data-ttu-id="b7d16-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b7d16-109">Type</span></span>   |<span data-ttu-id="b7d16-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b7d16-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7d16-111">address</span><span class="sxs-lookup"><span data-stu-id="b7d16-111">address</span></span>|<span data-ttu-id="b7d16-112">String</span><span class="sxs-lookup"><span data-stu-id="b7d16-112">String</span></span>|<span data-ttu-id="b7d16-113">Адрес электронной почты экземпляр сущности.</span><span class="sxs-lookup"><span data-stu-id="b7d16-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="b7d16-114">name</span><span class="sxs-lookup"><span data-stu-id="b7d16-114">name</span></span>|<span data-ttu-id="b7d16-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b7d16-115">String</span></span>|<span data-ttu-id="b7d16-116">Отображаемое имя экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b7d16-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7d16-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7d16-117">JSON representation</span></span>

<span data-ttu-id="b7d16-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7d16-118">Here is a JSON representation of the resource</span></span>

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

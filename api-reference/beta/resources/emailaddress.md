---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0ba6a1d67db75ce5c08654d74e959e08d529a0e7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457070"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="f734f-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="f734f-103">emailAddress resource type</span></span>

<span data-ttu-id="f734f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f734f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f734f-105">Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="f734f-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="f734f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f734f-106">Properties</span></span>
| <span data-ttu-id="f734f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f734f-107">Property</span></span>     | <span data-ttu-id="f734f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f734f-108">Type</span></span>   |<span data-ttu-id="f734f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f734f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f734f-110">address</span><span class="sxs-lookup"><span data-stu-id="f734f-110">address</span></span>|<span data-ttu-id="f734f-111">String</span><span class="sxs-lookup"><span data-stu-id="f734f-111">String</span></span>|<span data-ttu-id="f734f-112">Адрес электронной почты экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="f734f-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="f734f-113">name</span><span class="sxs-lookup"><span data-stu-id="f734f-113">name</span></span>|<span data-ttu-id="f734f-114">String</span><span class="sxs-lookup"><span data-stu-id="f734f-114">String</span></span>|<span data-ttu-id="f734f-115">Отображаемое имя экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="f734f-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f734f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f734f-116">JSON representation</span></span>

<span data-ttu-id="f734f-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f734f-117">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

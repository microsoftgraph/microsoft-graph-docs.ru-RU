---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4f0b36d84ffba5c5a8e39bd7603f92c815cda008
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972217"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="52a08-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="52a08-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52a08-104">Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="52a08-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="52a08-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="52a08-105">Properties</span></span>
| <span data-ttu-id="52a08-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="52a08-106">Property</span></span>     | <span data-ttu-id="52a08-107">Тип</span><span class="sxs-lookup"><span data-stu-id="52a08-107">Type</span></span>   |<span data-ttu-id="52a08-108">Описание</span><span class="sxs-lookup"><span data-stu-id="52a08-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52a08-109">address</span><span class="sxs-lookup"><span data-stu-id="52a08-109">address</span></span>|<span data-ttu-id="52a08-110">String</span><span class="sxs-lookup"><span data-stu-id="52a08-110">String</span></span>|<span data-ttu-id="52a08-111">Адрес электронной почты экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="52a08-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="52a08-112">name</span><span class="sxs-lookup"><span data-stu-id="52a08-112">name</span></span>|<span data-ttu-id="52a08-113">String</span><span class="sxs-lookup"><span data-stu-id="52a08-113">String</span></span>|<span data-ttu-id="52a08-114">Отображаемое имя экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="52a08-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52a08-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52a08-115">JSON representation</span></span>

<span data-ttu-id="52a08-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52a08-116">Here is a JSON representation of the resource</span></span>

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

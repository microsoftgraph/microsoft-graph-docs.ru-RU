---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d2a43300922ddf88df908d39d82b6efde2369348
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979492"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="98d03-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="98d03-103">emailAddress resource type</span></span>

<span data-ttu-id="98d03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d03-105">Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="98d03-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="98d03-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="98d03-106">Properties</span></span>
| <span data-ttu-id="98d03-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="98d03-107">Property</span></span>     | <span data-ttu-id="98d03-108">Тип</span><span class="sxs-lookup"><span data-stu-id="98d03-108">Type</span></span>   |<span data-ttu-id="98d03-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98d03-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98d03-110">address</span><span class="sxs-lookup"><span data-stu-id="98d03-110">address</span></span>|<span data-ttu-id="98d03-111">String</span><span class="sxs-lookup"><span data-stu-id="98d03-111">String</span></span>|<span data-ttu-id="98d03-112">Адрес электронной почты экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="98d03-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="98d03-113">name</span><span class="sxs-lookup"><span data-stu-id="98d03-113">name</span></span>|<span data-ttu-id="98d03-114">String</span><span class="sxs-lookup"><span data-stu-id="98d03-114">String</span></span>|<span data-ttu-id="98d03-115">Отображаемое имя экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="98d03-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98d03-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98d03-116">JSON representation</span></span>

<span data-ttu-id="98d03-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98d03-117">Here is a JSON representation of the resource</span></span>

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



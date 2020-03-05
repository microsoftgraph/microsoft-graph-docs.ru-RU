---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e0df635fb930816fa29b0d7f75a2075759a4c54d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499563"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="53425-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="53425-103">emailAddress resource type</span></span>

<span data-ttu-id="53425-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="53425-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53425-105">Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="53425-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="53425-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="53425-106">Properties</span></span>
| <span data-ttu-id="53425-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="53425-107">Property</span></span>     | <span data-ttu-id="53425-108">Тип</span><span class="sxs-lookup"><span data-stu-id="53425-108">Type</span></span>   |<span data-ttu-id="53425-109">Описание</span><span class="sxs-lookup"><span data-stu-id="53425-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53425-110">address</span><span class="sxs-lookup"><span data-stu-id="53425-110">address</span></span>|<span data-ttu-id="53425-111">String</span><span class="sxs-lookup"><span data-stu-id="53425-111">String</span></span>|<span data-ttu-id="53425-112">Адрес электронной почты экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="53425-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="53425-113">name</span><span class="sxs-lookup"><span data-stu-id="53425-113">name</span></span>|<span data-ttu-id="53425-114">String</span><span class="sxs-lookup"><span data-stu-id="53425-114">String</span></span>|<span data-ttu-id="53425-115">Отображаемое имя экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="53425-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53425-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53425-116">JSON representation</span></span>

<span data-ttu-id="53425-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53425-117">Here is a JSON representation of the resource</span></span>

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

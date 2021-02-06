---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра сущности, например получателя сообщения или владельца календаря.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8f572058d50672a26b3930f90a7b0492f9aa1eca
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132561"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="5a057-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="5a057-103">emailAddress resource type</span></span>

<span data-ttu-id="5a057-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a057-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a057-105">Представляет имя и SMTP-адрес экземпляра сущности, например получателя сообщения или владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="5a057-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="5a057-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a057-106">Properties</span></span>
| <span data-ttu-id="5a057-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a057-107">Property</span></span>     | <span data-ttu-id="5a057-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5a057-108">Type</span></span>   |<span data-ttu-id="5a057-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a057-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a057-110">address</span><span class="sxs-lookup"><span data-stu-id="5a057-110">address</span></span>|<span data-ttu-id="5a057-111">String</span><span class="sxs-lookup"><span data-stu-id="5a057-111">String</span></span>|<span data-ttu-id="5a057-112">Адрес электронной почты экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5a057-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="5a057-113">name</span><span class="sxs-lookup"><span data-stu-id="5a057-113">name</span></span>|<span data-ttu-id="5a057-114">String</span><span class="sxs-lookup"><span data-stu-id="5a057-114">String</span></span>|<span data-ttu-id="5a057-115">Отображаемого имени экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5a057-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a057-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5a057-116">JSON representation</span></span>

<span data-ttu-id="5a057-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a057-117">Here is a JSON representation of the resource</span></span>

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



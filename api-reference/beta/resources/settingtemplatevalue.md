---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9a49dd291bd9cc7baa31d90ba8e247ac984b1906
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965189"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="d29bd-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="d29bd-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d29bd-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="d29bd-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="d29bd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d29bd-105">Properties</span></span>
| <span data-ttu-id="d29bd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d29bd-106">Property</span></span>     | <span data-ttu-id="d29bd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d29bd-107">Type</span></span>   |<span data-ttu-id="d29bd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d29bd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d29bd-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d29bd-109">defaultValue</span></span>|<span data-ttu-id="d29bd-110">string</span><span class="sxs-lookup"><span data-stu-id="d29bd-110">string</span></span>|<span data-ttu-id="d29bd-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="d29bd-111">Default value for the setting.</span></span> <span data-ttu-id="d29bd-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d29bd-112">Read-only.</span></span>|
|<span data-ttu-id="d29bd-113">description</span><span class="sxs-lookup"><span data-stu-id="d29bd-113">description</span></span>|<span data-ttu-id="d29bd-114">string</span><span class="sxs-lookup"><span data-stu-id="d29bd-114">string</span></span>|<span data-ttu-id="d29bd-115">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="d29bd-115">Description of the setting.</span></span> <span data-ttu-id="d29bd-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d29bd-116">Read-only.</span></span>|
|<span data-ttu-id="d29bd-117">name</span><span class="sxs-lookup"><span data-stu-id="d29bd-117">name</span></span>|<span data-ttu-id="d29bd-118">строка</span><span class="sxs-lookup"><span data-stu-id="d29bd-118">string</span></span>|<span data-ttu-id="d29bd-119">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="d29bd-119">Name of the setting.</span></span> <span data-ttu-id="d29bd-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d29bd-120">Read-only.</span></span>|
|<span data-ttu-id="d29bd-121">type</span><span class="sxs-lookup"><span data-stu-id="d29bd-121">type</span></span>|<span data-ttu-id="d29bd-122">string</span><span class="sxs-lookup"><span data-stu-id="d29bd-122">string</span></span>|<span data-ttu-id="d29bd-123">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="d29bd-123">Type of the setting.</span></span> <span data-ttu-id="d29bd-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d29bd-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d29bd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d29bd-125">JSON representation</span></span>

<span data-ttu-id="d29bd-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d29bd-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

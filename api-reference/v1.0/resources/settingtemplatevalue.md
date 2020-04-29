---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eea9f77b26ee0ce88e2c97c87e7cca50cbf48491
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533745"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="acece-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="acece-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="acece-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acece-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="acece-105">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="acece-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="acece-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="acece-106">Properties</span></span>

| <span data-ttu-id="acece-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="acece-107">Property</span></span> | <span data-ttu-id="acece-108">Тип</span><span class="sxs-lookup"><span data-stu-id="acece-108">Type</span></span> | <span data-ttu-id="acece-109">Описание</span><span class="sxs-lookup"><span data-stu-id="acece-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="acece-110">Значение</span><span class="sxs-lookup"><span data-stu-id="acece-110">defaultValue</span></span>|<span data-ttu-id="acece-111">String</span><span class="sxs-lookup"><span data-stu-id="acece-111">String</span></span>| <span data-ttu-id="acece-112">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="acece-112">Default value for the setting.</span></span> |
|<span data-ttu-id="acece-113">description</span><span class="sxs-lookup"><span data-stu-id="acece-113">description</span></span>|<span data-ttu-id="acece-114">String</span><span class="sxs-lookup"><span data-stu-id="acece-114">String</span></span>| <span data-ttu-id="acece-115">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="acece-115">Description of the setting.</span></span> |
|<span data-ttu-id="acece-116">name</span><span class="sxs-lookup"><span data-stu-id="acece-116">name</span></span>|<span data-ttu-id="acece-117">String</span><span class="sxs-lookup"><span data-stu-id="acece-117">String</span></span>| <span data-ttu-id="acece-118">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="acece-118">Name of the setting.</span></span> |
|<span data-ttu-id="acece-119">type</span><span class="sxs-lookup"><span data-stu-id="acece-119">type</span></span>|<span data-ttu-id="acece-120">String</span><span class="sxs-lookup"><span data-stu-id="acece-120">String</span></span>| <span data-ttu-id="acece-121">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="acece-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="acece-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="acece-122">JSON representation</span></span>

<span data-ttu-id="acece-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acece-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549694"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="9a815-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="9a815-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="9a815-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="9a815-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="9a815-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a815-105">Properties</span></span>

| <span data-ttu-id="9a815-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a815-106">Property</span></span> | <span data-ttu-id="9a815-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9a815-107">Type</span></span> | <span data-ttu-id="9a815-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9a815-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9a815-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9a815-109">defaultValue</span></span>|<span data-ttu-id="9a815-110">String</span><span class="sxs-lookup"><span data-stu-id="9a815-110">String</span></span>| <span data-ttu-id="9a815-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="9a815-111">Default value for the setting.</span></span> |
|<span data-ttu-id="9a815-112">description</span><span class="sxs-lookup"><span data-stu-id="9a815-112">description</span></span>|<span data-ttu-id="9a815-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9a815-113">String</span></span>| <span data-ttu-id="9a815-114">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="9a815-114">Description of the setting.</span></span> |
|<span data-ttu-id="9a815-115">name</span><span class="sxs-lookup"><span data-stu-id="9a815-115">name</span></span>|<span data-ttu-id="9a815-116">String</span><span class="sxs-lookup"><span data-stu-id="9a815-116">String</span></span>| <span data-ttu-id="9a815-117">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="9a815-117">Name of the setting.</span></span> |
|<span data-ttu-id="9a815-118">type</span><span class="sxs-lookup"><span data-stu-id="9a815-118">type</span></span>|<span data-ttu-id="9a815-119">String</span><span class="sxs-lookup"><span data-stu-id="9a815-119">String</span></span>| <span data-ttu-id="9a815-120">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="9a815-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="9a815-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9a815-121">JSON representation</span></span>

<span data-ttu-id="9a815-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a815-122">Here is a JSON representation of the resource.</span></span>

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

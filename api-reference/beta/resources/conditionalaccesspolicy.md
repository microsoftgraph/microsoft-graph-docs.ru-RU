---
title: Тип ресурса Кондитионалакцессполици
description: Указывает атрибуты, связанные с политикой условного доступа или политиками, активируемыми соответствующими действиями при входе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2c45be8ee32c26187ccf42154ba6c06b60f5efc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973218"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="4e200-103">Тип ресурса Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="4e200-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="4e200-104">Указывает атрибуты, связанные с политикой условного доступа или политиками, активируемыми соответствующими действиями при входе.</span><span class="sxs-lookup"><span data-stu-id="4e200-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="4e200-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e200-105">Properties</span></span>
| <span data-ttu-id="4e200-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e200-106">Property</span></span>     | <span data-ttu-id="4e200-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4e200-107">Type</span></span>   |<span data-ttu-id="4e200-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4e200-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e200-109">displayName</span><span class="sxs-lookup"><span data-stu-id="4e200-109">displayName</span></span>|<span data-ttu-id="4e200-110">Строка</span><span class="sxs-lookup"><span data-stu-id="4e200-110">String</span></span>|<span data-ttu-id="4e200-111">Указывает имя политики условного доступа (пример: "требовать MFA для Salesforce").</span><span class="sxs-lookup"><span data-stu-id="4e200-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="4e200-112">Енфорцедгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="4e200-112">enforcedGrantControls</span></span>|<span data-ttu-id="4e200-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4e200-113">String collection</span></span>|<span data-ttu-id="4e200-114">Указывает на элементы управления предоставлением, принудительно примененные политикой условного доступа (пример: "требовать многофакторную проверку подлинности").</span><span class="sxs-lookup"><span data-stu-id="4e200-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="4e200-115">Енфорцедсессионконтролс</span><span class="sxs-lookup"><span data-stu-id="4e200-115">enforcedSessionControls</span></span>|<span data-ttu-id="4e200-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4e200-116">String collection</span></span>|<span data-ttu-id="4e200-117">Указывает на элементы управления сеансом, принудительно примененные политикой условного доступа (пример: "требовать принудительно заданное приложением элементов управления").</span><span class="sxs-lookup"><span data-stu-id="4e200-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="4e200-118">id</span><span class="sxs-lookup"><span data-stu-id="4e200-118">id</span></span>|<span data-ttu-id="4e200-119">String</span><span class="sxs-lookup"><span data-stu-id="4e200-119">String</span></span>|<span data-ttu-id="4e200-120">Уникальный идентификатор GUID политики условного доступа</span><span class="sxs-lookup"><span data-stu-id="4e200-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="4e200-121">result</span><span class="sxs-lookup"><span data-stu-id="4e200-121">result</span></span>|<span data-ttu-id="4e200-122">String</span><span class="sxs-lookup"><span data-stu-id="4e200-122">String</span></span>| <span data-ttu-id="4e200-123">Указывает результат политики ЦС, который был активирован. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="4e200-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="4e200-124">`notApplied`-Политика не применяется, так как условия политики не выполнены.</span><span class="sxs-lookup"><span data-stu-id="4e200-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="4e200-125">`notEnabled`— Это связано с тем, что в отключенном состоянии политика отключена.</span><span class="sxs-lookup"><span data-stu-id="4e200-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e200-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e200-126">JSON representation</span></span>

<span data-ttu-id="4e200-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e200-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

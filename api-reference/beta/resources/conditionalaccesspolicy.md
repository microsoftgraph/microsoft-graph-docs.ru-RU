---
title: Тип ресурса Кондитионалакцессполици
description: Указывает атрибуты, связанные с политикой условного доступа или политиками, активируемыми соответствующими действиями при входе.
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543373"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="b8170-103">Тип ресурса Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="b8170-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="b8170-104">Указывает атрибуты, связанные с политикой условного доступа или политиками, активируемыми соответствующими действиями при входе.</span><span class="sxs-lookup"><span data-stu-id="b8170-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="b8170-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8170-105">Properties</span></span>
| <span data-ttu-id="b8170-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8170-106">Property</span></span>     | <span data-ttu-id="b8170-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b8170-107">Type</span></span>   |<span data-ttu-id="b8170-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b8170-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8170-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b8170-109">displayName</span></span>|<span data-ttu-id="b8170-110">String</span><span class="sxs-lookup"><span data-stu-id="b8170-110">String</span></span>|<span data-ttu-id="b8170-111">Указывает имя политики условного доступа (пример: "требовать MFA для Salesforce").</span><span class="sxs-lookup"><span data-stu-id="b8170-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="b8170-112">Енфорцедгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="b8170-112">enforcedGrantControls</span></span>|<span data-ttu-id="b8170-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b8170-113">String collection</span></span>|<span data-ttu-id="b8170-114">Указывает на элементы управления предоставлением, принудительно примененные политикой условного доступа (пример: "требовать многофакторную проверку подлинности").</span><span class="sxs-lookup"><span data-stu-id="b8170-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="b8170-115">Енфорцедсессионконтролс</span><span class="sxs-lookup"><span data-stu-id="b8170-115">enforcedSessionControls</span></span>|<span data-ttu-id="b8170-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b8170-116">String collection</span></span>|<span data-ttu-id="b8170-117">Указывает на элементы управления сеансом, принудительно примененные политикой условного доступа (пример: "требовать принудительно заданное приложением элементов управления").</span><span class="sxs-lookup"><span data-stu-id="b8170-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="b8170-118">id</span><span class="sxs-lookup"><span data-stu-id="b8170-118">id</span></span>|<span data-ttu-id="b8170-119">String</span><span class="sxs-lookup"><span data-stu-id="b8170-119">String</span></span>|<span data-ttu-id="b8170-120">Уникальный идентификатор GUID политики условного доступа</span><span class="sxs-lookup"><span data-stu-id="b8170-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="b8170-121">result</span><span class="sxs-lookup"><span data-stu-id="b8170-121">result</span></span>|<span data-ttu-id="b8170-122">String</span><span class="sxs-lookup"><span data-stu-id="b8170-122">String</span></span>| <span data-ttu-id="b8170-123">Указывает результат политики ЦС, который был активирован. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="b8170-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="b8170-124">`notApplied`-Политика не применяется, так как условия политики не выполнены.</span><span class="sxs-lookup"><span data-stu-id="b8170-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="b8170-125">`notEnabled`— Это связано с тем, что в отключенном состоянии политика отключена.</span><span class="sxs-lookup"><span data-stu-id="b8170-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8170-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b8170-126">JSON representation</span></span>

<span data-ttu-id="b8170-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8170-127">Here is a JSON representation of the resource.</span></span>

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

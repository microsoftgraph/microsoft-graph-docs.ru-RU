---
title: Тип ресурса conditionalAccessPolicy
description: Указывает, что атрибуты, связанные с условного доступа политики или политики запускаются с соответствующей операции регистрации
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820645"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="781f4-103">Тип ресурса conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="781f4-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="781f4-104">Указывает, что атрибуты, связанные с условного доступа политики или политики запускаются с соответствующей операции регистрации</span><span class="sxs-lookup"><span data-stu-id="781f4-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="781f4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="781f4-105">Properties</span></span>
| <span data-ttu-id="781f4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="781f4-106">Property</span></span>     | <span data-ttu-id="781f4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="781f4-107">Type</span></span>   |<span data-ttu-id="781f4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="781f4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="781f4-109">displayName</span><span class="sxs-lookup"><span data-stu-id="781f4-109">displayName</span></span>|<span data-ttu-id="781f4-110">Строка</span><span class="sxs-lookup"><span data-stu-id="781f4-110">String</span></span>|<span data-ttu-id="781f4-111">— Это имя политики условного доступа (пример: «Требовать многофакторной проверкой Подлинности для Salesforce»).</span><span class="sxs-lookup"><span data-stu-id="781f4-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="781f4-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="781f4-112">enforcedGrantControls</span></span>|<span data-ttu-id="781f4-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="781f4-113">String collection</span></span>|<span data-ttu-id="781f4-114">Относится к элементам управления grant, определяемое политики условного доступа (пример: «Требовать многофакторной проверки подлинности»).</span><span class="sxs-lookup"><span data-stu-id="781f4-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="781f4-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="781f4-115">enforcedSessionControls</span></span>|<span data-ttu-id="781f4-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="781f4-116">String collection</span></span>|<span data-ttu-id="781f4-117">Относится к элементам управления сеанса, определяемое политики условного доступа (пример: «Требовать применения приложения элементы управления»).</span><span class="sxs-lookup"><span data-stu-id="781f4-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="781f4-118">id</span><span class="sxs-lookup"><span data-stu-id="781f4-118">id</span></span>|<span data-ttu-id="781f4-119">Строка</span><span class="sxs-lookup"><span data-stu-id="781f4-119">String</span></span>|<span data-ttu-id="781f4-120">Уникальный идентификатор GUID политики условного доступа</span><span class="sxs-lookup"><span data-stu-id="781f4-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="781f4-121">result</span><span class="sxs-lookup"><span data-stu-id="781f4-121">result</span></span>|<span data-ttu-id="781f4-122">Строка</span><span class="sxs-lookup"><span data-stu-id="781f4-122">String</span></span>| <span data-ttu-id="781f4-123">Указывает результат политики центра сертификации, который был активирован. Возможными значениями являются:</span><span class="sxs-lookup"><span data-stu-id="781f4-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="781f4-124">`notApplied`-Политики не применяется, так как не были выполнены условия политики.</span><span class="sxs-lookup"><span data-stu-id="781f4-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="781f4-125">`notEnabled`— Это из-за политики в отключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="781f4-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="781f4-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="781f4-126">JSON representation</span></span>

<span data-ttu-id="781f4-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="781f4-127">Here is a JSON representation of the resource.</span></span>

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

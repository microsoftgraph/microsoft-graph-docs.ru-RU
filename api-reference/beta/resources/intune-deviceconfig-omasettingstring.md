---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
ms.openlocfilehash: e0137a3d1ce7d950c107c7a63e0e5a399b3bf6d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077991"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="55737-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="55737-103">omaSettingString resource type</span></span>

> <span data-ttu-id="55737-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="55737-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55737-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55737-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55737-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="55737-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55737-107">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="55737-107">OMA Settings String definition.</span></span>

<span data-ttu-id="55737-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="55737-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55737-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="55737-109">Properties</span></span>
|<span data-ttu-id="55737-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="55737-110">Property</span></span>|<span data-ttu-id="55737-111">Тип</span><span class="sxs-lookup"><span data-stu-id="55737-111">Type</span></span>|<span data-ttu-id="55737-112">Описание</span><span class="sxs-lookup"><span data-stu-id="55737-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55737-113">displayName</span><span class="sxs-lookup"><span data-stu-id="55737-113">displayName</span></span>|<span data-ttu-id="55737-114">String</span><span class="sxs-lookup"><span data-stu-id="55737-114">String</span></span>|<span data-ttu-id="55737-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="55737-115">Display Name.</span></span> <span data-ttu-id="55737-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="55737-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="55737-117">описание</span><span class="sxs-lookup"><span data-stu-id="55737-117">description</span></span>|<span data-ttu-id="55737-118">String</span><span class="sxs-lookup"><span data-stu-id="55737-118">String</span></span>|<span data-ttu-id="55737-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="55737-119">Description.</span></span> <span data-ttu-id="55737-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="55737-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="55737-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="55737-121">omaUri</span></span>|<span data-ttu-id="55737-122">String</span><span class="sxs-lookup"><span data-stu-id="55737-122">String</span></span>|<span data-ttu-id="55737-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="55737-123">OMA.</span></span> <span data-ttu-id="55737-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="55737-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="55737-125">value</span><span class="sxs-lookup"><span data-stu-id="55737-125">value</span></span>|<span data-ttu-id="55737-126">String</span><span class="sxs-lookup"><span data-stu-id="55737-126">String</span></span>|<span data-ttu-id="55737-127">Значение</span><span class="sxs-lookup"><span data-stu-id="55737-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55737-128">Связи</span><span class="sxs-lookup"><span data-stu-id="55737-128">Relationships</span></span>
<span data-ttu-id="55737-129">Нет</span><span class="sxs-lookup"><span data-stu-id="55737-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55737-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55737-130">JSON Representation</span></span>
<span data-ttu-id="55737-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55737-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```






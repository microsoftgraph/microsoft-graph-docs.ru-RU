---
title: Тип ресурса Девицеманажементсеттингпрофилеконстраинт
description: Ограничение на применение заданной метаданных профиля
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 917483556c71853856ff8b70973167b2c749a3a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267966"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="46a39-103">Тип ресурса Девицеманажементсеттингпрофилеконстраинт</span><span class="sxs-lookup"><span data-stu-id="46a39-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="46a39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46a39-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46a39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46a39-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46a39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46a39-107">Ограничение на применение заданной метаданных профиля</span><span class="sxs-lookup"><span data-stu-id="46a39-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="46a39-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="46a39-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46a39-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="46a39-109">Properties</span></span>
|<span data-ttu-id="46a39-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="46a39-110">Property</span></span>|<span data-ttu-id="46a39-111">Тип</span><span class="sxs-lookup"><span data-stu-id="46a39-111">Type</span></span>|<span data-ttu-id="46a39-112">Описание</span><span class="sxs-lookup"><span data-stu-id="46a39-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46a39-113">source</span><span class="sxs-lookup"><span data-stu-id="46a39-113">source</span></span>|<span data-ttu-id="46a39-114">String</span><span class="sxs-lookup"><span data-stu-id="46a39-114">String</span></span>|<span data-ttu-id="46a39-115">Источник объекта</span><span class="sxs-lookup"><span data-stu-id="46a39-115">The source of the entity</span></span>|
|<span data-ttu-id="46a39-116">types</span><span class="sxs-lookup"><span data-stu-id="46a39-116">types</span></span>|<span data-ttu-id="46a39-117">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="46a39-117">String collection</span></span>|<span data-ttu-id="46a39-118">Коллекция типов, которые несет данный объект</span><span class="sxs-lookup"><span data-stu-id="46a39-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="46a39-119">Связи</span><span class="sxs-lookup"><span data-stu-id="46a39-119">Relationships</span></span>
<span data-ttu-id="46a39-120">Нет</span><span class="sxs-lookup"><span data-stu-id="46a39-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46a39-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46a39-121">JSON Representation</span></span>
<span data-ttu-id="46a39-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46a39-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingProfileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingProfileConstraint",
  "source": "String",
  "types": [
    "String"
  ]
}
```





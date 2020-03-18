---
title: Тип ресурса Девицеманажементсеттингпрофилеконстраинт
description: Ограничение на применение заданной метаданных профиля
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4b565321069c27949fbd5814c4ddc1c4eb1451b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785304"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="c806c-103">Тип ресурса Девицеманажементсеттингпрофилеконстраинт</span><span class="sxs-lookup"><span data-stu-id="c806c-103">deviceManagementSettingProfileConstraint resource type</span></span>

> <span data-ttu-id="c806c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c806c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c806c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c806c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c806c-106">Ограничение на применение заданной метаданных профиля</span><span class="sxs-lookup"><span data-stu-id="c806c-106">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="c806c-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="c806c-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c806c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c806c-108">Properties</span></span>
|<span data-ttu-id="c806c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c806c-109">Property</span></span>|<span data-ttu-id="c806c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c806c-110">Type</span></span>|<span data-ttu-id="c806c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c806c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c806c-112">source</span><span class="sxs-lookup"><span data-stu-id="c806c-112">source</span></span>|<span data-ttu-id="c806c-113">String</span><span class="sxs-lookup"><span data-stu-id="c806c-113">String</span></span>|<span data-ttu-id="c806c-114">Источник объекта</span><span class="sxs-lookup"><span data-stu-id="c806c-114">The source of the entity</span></span>|
|<span data-ttu-id="c806c-115">types</span><span class="sxs-lookup"><span data-stu-id="c806c-115">types</span></span>|<span data-ttu-id="c806c-116">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c806c-116">String collection</span></span>|<span data-ttu-id="c806c-117">Коллекция типов, которые несет данный объект</span><span class="sxs-lookup"><span data-stu-id="c806c-117">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="c806c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c806c-118">Relationships</span></span>
<span data-ttu-id="c806c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c806c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c806c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c806c-120">JSON Representation</span></span>
<span data-ttu-id="c806c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c806c-121">Here is a JSON representation of the resource.</span></span>
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




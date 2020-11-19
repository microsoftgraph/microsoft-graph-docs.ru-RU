---
title: Тип ресурса Девицеманажементконфигуратионсеттингдепендедонби
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3d9b6bde7217460867ab7e9b77853fcb366e38c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242184"
---
# <a name="devicemanagementconfigurationsettingdependedonby-resource-type"></a><span data-ttu-id="a17ce-103">Тип ресурса Девицеманажементконфигуратионсеттингдепендедонби</span><span class="sxs-lookup"><span data-stu-id="a17ce-103">deviceManagementConfigurationSettingDependedOnBy resource type</span></span>

<span data-ttu-id="a17ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a17ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a17ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a17ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a17ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a17ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a17ce-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a17ce-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a17ce-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a17ce-108">Properties</span></span>
|<span data-ttu-id="a17ce-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a17ce-109">Property</span></span>|<span data-ttu-id="a17ce-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a17ce-110">Type</span></span>|<span data-ttu-id="a17ce-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a17ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a17ce-112">депендедонби</span><span class="sxs-lookup"><span data-stu-id="a17ce-112">dependedOnBy</span></span>|<span data-ttu-id="a17ce-113">String</span><span class="sxs-lookup"><span data-stu-id="a17ce-113">String</span></span>|<span data-ttu-id="a17ce-114">Идентификатор параметра дочернего объекта, зависящий от текущего параметра</span><span class="sxs-lookup"><span data-stu-id="a17ce-114">Identifier of child setting that is dependent on the current setting</span></span>|
|<span data-ttu-id="a17ce-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="a17ce-115">required</span></span>|<span data-ttu-id="a17ce-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a17ce-116">Boolean</span></span>|<span data-ttu-id="a17ce-117">Значение, определяющее, является ли параметр дочернего элемента обязательным в зависимости от выбора родительского параметра</span><span class="sxs-lookup"><span data-stu-id="a17ce-117">Value that determines if the child setting is required based on the parent setting's selection</span></span>|

## <a name="relationships"></a><span data-ttu-id="a17ce-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a17ce-118">Relationships</span></span>
<span data-ttu-id="a17ce-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a17ce-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a17ce-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a17ce-120">JSON Representation</span></span>
<span data-ttu-id="a17ce-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a17ce-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
  "dependedOnBy": "String",
  "required": true
}
```





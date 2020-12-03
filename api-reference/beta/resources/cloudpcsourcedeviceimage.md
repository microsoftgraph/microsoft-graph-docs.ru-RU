---
title: Тип ресурса Клаудпксаурцедевицеимаже
description: 'Исходное изображение, связанное с вашей подпиской Azure. '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c944ab1a634d10e978c6ce1620ebe1accc5e4359
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563746"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a><span data-ttu-id="c5d60-103">Тип ресурса Клаудпксаурцедевицеимаже</span><span class="sxs-lookup"><span data-stu-id="c5d60-103">cloudPcSourceDeviceImage resource type</span></span>

<span data-ttu-id="c5d60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5d60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5d60-105">Исходное изображение, связанное с вашей подпиской Azure.</span><span class="sxs-lookup"><span data-stu-id="c5d60-105">The source image associated with your Azure subscription.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="c5d60-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5d60-106">Properties</span></span>

|<span data-ttu-id="c5d60-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5d60-107">Property</span></span>|<span data-ttu-id="c5d60-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c5d60-108">Type</span></span>|<span data-ttu-id="c5d60-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c5d60-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d60-110">id</span><span class="sxs-lookup"><span data-stu-id="c5d60-110">id</span></span>|<span data-ttu-id="c5d60-111">String</span><span class="sxs-lookup"><span data-stu-id="c5d60-111">String</span></span>|<span data-ttu-id="c5d60-112">Идентификатор исходного изображения.</span><span class="sxs-lookup"><span data-stu-id="c5d60-112">The ID of the source image.</span></span>|
|<span data-ttu-id="c5d60-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c5d60-113">displayName</span></span>|<span data-ttu-id="c5d60-114">String</span><span class="sxs-lookup"><span data-stu-id="c5d60-114">String</span></span>|<span data-ttu-id="c5d60-115">Отображаемое имя исходного изображения.</span><span class="sxs-lookup"><span data-stu-id="c5d60-115">The display name for the source image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5d60-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c5d60-116">Relationships</span></span>

<span data-ttu-id="c5d60-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c5d60-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5d60-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c5d60-118">JSON representation</span></span>

<span data-ttu-id="c5d60-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5d60-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage",
  "baseType": "microsoft.graph.entity"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```

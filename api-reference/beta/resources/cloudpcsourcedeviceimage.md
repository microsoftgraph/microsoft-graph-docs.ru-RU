---
title: Тип ресурса cloudPcSourceDeviceImage
description: 'Исходный образ, связанный с подпиской на Azure. '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b0c656142ddad5af3d0af7778d0ae04f0c5d7b4
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790743"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a><span data-ttu-id="208b8-103">Тип ресурса cloudPcSourceDeviceImage</span><span class="sxs-lookup"><span data-stu-id="208b8-103">cloudPcSourceDeviceImage resource type</span></span>

<span data-ttu-id="208b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="208b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="208b8-105">Исходный образ, связанный с подпиской на Azure.</span><span class="sxs-lookup"><span data-stu-id="208b8-105">The source image associated with your Azure subscription.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="208b8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="208b8-106">Properties</span></span>

|<span data-ttu-id="208b8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="208b8-107">Property</span></span>|<span data-ttu-id="208b8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="208b8-108">Type</span></span>|<span data-ttu-id="208b8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="208b8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="208b8-110">id</span><span class="sxs-lookup"><span data-stu-id="208b8-110">id</span></span>|<span data-ttu-id="208b8-111">String</span><span class="sxs-lookup"><span data-stu-id="208b8-111">String</span></span>|<span data-ttu-id="208b8-112">ИД изображения источника.</span><span class="sxs-lookup"><span data-stu-id="208b8-112">The ID of the source image.</span></span>|
|<span data-ttu-id="208b8-113">displayName</span><span class="sxs-lookup"><span data-stu-id="208b8-113">displayName</span></span>|<span data-ttu-id="208b8-114">String</span><span class="sxs-lookup"><span data-stu-id="208b8-114">String</span></span>|<span data-ttu-id="208b8-115">Отображаемая имя для изображения источника.</span><span class="sxs-lookup"><span data-stu-id="208b8-115">The display name for the source image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="208b8-116">Связи</span><span class="sxs-lookup"><span data-stu-id="208b8-116">Relationships</span></span>

<span data-ttu-id="208b8-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="208b8-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="208b8-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="208b8-118">JSON representation</span></span>

<span data-ttu-id="208b8-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="208b8-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```

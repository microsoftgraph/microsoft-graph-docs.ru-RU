---
title: Тип ресурса Девицелогколлектионрекуест
description: Сущность запроса для сбора журналов Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f48e8511f7cbce95e15b1816831a471207c1558a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299333"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="e9f9b-103">Тип ресурса Девицелогколлектионрекуест</span><span class="sxs-lookup"><span data-stu-id="e9f9b-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="e9f9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9f9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9f9b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9f9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9f9b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9f9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9f9b-107">Сущность запроса для сбора журналов Windows.</span><span class="sxs-lookup"><span data-stu-id="e9f9b-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="e9f9b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9f9b-108">Properties</span></span>
|<span data-ttu-id="e9f9b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9f9b-109">Property</span></span>|<span data-ttu-id="e9f9b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e9f9b-110">Type</span></span>|<span data-ttu-id="e9f9b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e9f9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f9b-112">id</span><span class="sxs-lookup"><span data-stu-id="e9f9b-112">id</span></span>|<span data-ttu-id="e9f9b-113">String</span><span class="sxs-lookup"><span data-stu-id="e9f9b-113">String</span></span>|<span data-ttu-id="e9f9b-114">Уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="e9f9b-114">The unique identifier</span></span>|
|<span data-ttu-id="e9f9b-115">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="e9f9b-115">templateType</span></span>|[<span data-ttu-id="e9f9b-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="e9f9b-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="e9f9b-117">Тип шаблона, отправляемый с запросом коллекции.</span><span class="sxs-lookup"><span data-stu-id="e9f9b-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="e9f9b-118">Возможные значения: `predefined` .</span><span class="sxs-lookup"><span data-stu-id="e9f9b-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9f9b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e9f9b-119">Relationships</span></span>
<span data-ttu-id="e9f9b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e9f9b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9f9b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9f9b-121">JSON Representation</span></span>
<span data-ttu-id="e9f9b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9f9b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String (identifier)",
  "templateType": "String"
}
```





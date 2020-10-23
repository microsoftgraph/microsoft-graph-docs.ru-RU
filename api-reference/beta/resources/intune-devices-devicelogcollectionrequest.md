---
title: Тип ресурса Девицелогколлектионрекуест
description: Сущность запроса для сбора журналов Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e0be1fabe16e51c9ca9840f2417bc1d70d67b39
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694972"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="c7696-103">Тип ресурса Девицелогколлектионрекуест</span><span class="sxs-lookup"><span data-stu-id="c7696-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="c7696-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7696-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7696-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7696-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7696-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7696-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7696-107">Сущность запроса для сбора журналов Windows.</span><span class="sxs-lookup"><span data-stu-id="c7696-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="c7696-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7696-108">Properties</span></span>
|<span data-ttu-id="c7696-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7696-109">Property</span></span>|<span data-ttu-id="c7696-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c7696-110">Type</span></span>|<span data-ttu-id="c7696-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7696-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7696-112">id</span><span class="sxs-lookup"><span data-stu-id="c7696-112">id</span></span>|<span data-ttu-id="c7696-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c7696-113">String</span></span>|<span data-ttu-id="c7696-114">Уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="c7696-114">The unique identifier</span></span>|
|<span data-ttu-id="c7696-115">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="c7696-115">templateType</span></span>|[<span data-ttu-id="c7696-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="c7696-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="c7696-117">Тип шаблона, отправляемый с запросом коллекции.</span><span class="sxs-lookup"><span data-stu-id="c7696-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="c7696-118">Возможные значения: `predefined` .</span><span class="sxs-lookup"><span data-stu-id="c7696-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7696-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c7696-119">Relationships</span></span>
<span data-ttu-id="c7696-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c7696-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7696-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7696-121">JSON Representation</span></span>
<span data-ttu-id="c7696-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7696-122">Here is a JSON representation of the resource.</span></span>
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






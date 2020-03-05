---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91e3cc0beec0a5854eb6c77a6510062614646900
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526453"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="746a8-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="746a8-103">extendedKeyUsage resource type</span></span>

<span data-ttu-id="746a8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="746a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="746a8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="746a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="746a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="746a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="746a8-107">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="746a8-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="746a8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="746a8-108">Properties</span></span>
|<span data-ttu-id="746a8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="746a8-109">Property</span></span>|<span data-ttu-id="746a8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="746a8-110">Type</span></span>|<span data-ttu-id="746a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="746a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="746a8-112">name</span><span class="sxs-lookup"><span data-stu-id="746a8-112">name</span></span>|<span data-ttu-id="746a8-113">String</span><span class="sxs-lookup"><span data-stu-id="746a8-113">String</span></span>|<span data-ttu-id="746a8-114">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="746a8-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="746a8-115">обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="746a8-115">objectIdentifier</span></span>|<span data-ttu-id="746a8-116">String</span><span class="sxs-lookup"><span data-stu-id="746a8-116">String</span></span>|<span data-ttu-id="746a8-117">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="746a8-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="746a8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="746a8-118">Relationships</span></span>
<span data-ttu-id="746a8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="746a8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="746a8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="746a8-120">JSON Representation</span></span>
<span data-ttu-id="746a8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="746a8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




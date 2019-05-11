---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36752e9a2f86e68bd4ada1a342dc174726a684c7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946954"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="cfad3-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="cfad3-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="cfad3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfad3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfad3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfad3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfad3-106">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="cfad3-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="cfad3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfad3-107">Properties</span></span>
|<span data-ttu-id="cfad3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfad3-108">Property</span></span>|<span data-ttu-id="cfad3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cfad3-109">Type</span></span>|<span data-ttu-id="cfad3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cfad3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfad3-111">name</span><span class="sxs-lookup"><span data-stu-id="cfad3-111">name</span></span>|<span data-ttu-id="cfad3-112">String</span><span class="sxs-lookup"><span data-stu-id="cfad3-112">String</span></span>|<span data-ttu-id="cfad3-113">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="cfad3-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="cfad3-114">Обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="cfad3-114">objectIdentifier</span></span>|<span data-ttu-id="cfad3-115">Строка</span><span class="sxs-lookup"><span data-stu-id="cfad3-115">String</span></span>|<span data-ttu-id="cfad3-116">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="cfad3-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfad3-117">Связи</span><span class="sxs-lookup"><span data-stu-id="cfad3-117">Relationships</span></span>
<span data-ttu-id="cfad3-118">Нет</span><span class="sxs-lookup"><span data-stu-id="cfad3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfad3-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfad3-119">JSON Representation</span></span>
<span data-ttu-id="cfad3-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfad3-120">Here is a JSON representation of the resource.</span></span>
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





---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd89a46c2739f80a0a5c661884fb5e72c6e17522
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789215"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="5cc8f-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="5cc8f-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="5cc8f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cc8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cc8f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5cc8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc8f-106">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="5cc8f-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="5cc8f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cc8f-107">Properties</span></span>
|<span data-ttu-id="5cc8f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cc8f-108">Property</span></span>|<span data-ttu-id="5cc8f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5cc8f-109">Type</span></span>|<span data-ttu-id="5cc8f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5cc8f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc8f-111">name</span><span class="sxs-lookup"><span data-stu-id="5cc8f-111">name</span></span>|<span data-ttu-id="5cc8f-112">String</span><span class="sxs-lookup"><span data-stu-id="5cc8f-112">String</span></span>|<span data-ttu-id="5cc8f-113">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="5cc8f-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="5cc8f-114">Обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="5cc8f-114">objectIdentifier</span></span>|<span data-ttu-id="5cc8f-115">String</span><span class="sxs-lookup"><span data-stu-id="5cc8f-115">String</span></span>|<span data-ttu-id="5cc8f-116">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="5cc8f-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cc8f-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="5cc8f-117">Relationships</span></span>
<span data-ttu-id="5cc8f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5cc8f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cc8f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cc8f-119">JSON Representation</span></span>
<span data-ttu-id="5cc8f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cc8f-120">Here is a JSON representation of the resource.</span></span>
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






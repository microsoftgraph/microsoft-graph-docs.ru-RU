---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d02154b9513e1ef3edac8cf823bd718d3e356691
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325584"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="f3dcd-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="f3dcd-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="f3dcd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3dcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3dcd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3dcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3dcd-106">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="f3dcd-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="f3dcd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3dcd-107">Properties</span></span>
|<span data-ttu-id="f3dcd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3dcd-108">Property</span></span>|<span data-ttu-id="f3dcd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3dcd-109">Type</span></span>|<span data-ttu-id="f3dcd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3dcd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3dcd-111">name</span><span class="sxs-lookup"><span data-stu-id="f3dcd-111">name</span></span>|<span data-ttu-id="f3dcd-112">String</span><span class="sxs-lookup"><span data-stu-id="f3dcd-112">String</span></span>|<span data-ttu-id="f3dcd-113">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="f3dcd-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="f3dcd-114">обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="f3dcd-114">objectIdentifier</span></span>|<span data-ttu-id="f3dcd-115">String</span><span class="sxs-lookup"><span data-stu-id="f3dcd-115">String</span></span>|<span data-ttu-id="f3dcd-116">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="f3dcd-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3dcd-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3dcd-117">Relationships</span></span>
<span data-ttu-id="f3dcd-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f3dcd-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3dcd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3dcd-119">JSON Representation</span></span>
<span data-ttu-id="f3dcd-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3dcd-120">Here is a JSON representation of the resource.</span></span>
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




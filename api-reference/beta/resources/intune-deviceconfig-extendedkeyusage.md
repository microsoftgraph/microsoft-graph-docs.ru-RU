---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4fe1818aca19053242882e45edd1da5bbc544e8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460037"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="3776e-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="3776e-103">extendedKeyUsage resource type</span></span>

<span data-ttu-id="3776e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3776e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3776e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3776e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3776e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3776e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3776e-107">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="3776e-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="3776e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3776e-108">Properties</span></span>
|<span data-ttu-id="3776e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3776e-109">Property</span></span>|<span data-ttu-id="3776e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3776e-110">Type</span></span>|<span data-ttu-id="3776e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3776e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3776e-112">name</span><span class="sxs-lookup"><span data-stu-id="3776e-112">name</span></span>|<span data-ttu-id="3776e-113">String</span><span class="sxs-lookup"><span data-stu-id="3776e-113">String</span></span>|<span data-ttu-id="3776e-114">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="3776e-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="3776e-115">обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="3776e-115">objectIdentifier</span></span>|<span data-ttu-id="3776e-116">String</span><span class="sxs-lookup"><span data-stu-id="3776e-116">String</span></span>|<span data-ttu-id="3776e-117">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="3776e-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="3776e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3776e-118">Relationships</span></span>
<span data-ttu-id="3776e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3776e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3776e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3776e-120">JSON Representation</span></span>
<span data-ttu-id="3776e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3776e-121">Here is a JSON representation of the resource.</span></span>
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




---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9478750010597f30ae19801b1e40659dd3247ac
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302071"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="4e5b5-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="4e5b5-103">extendedKeyUsage resource type</span></span>

<span data-ttu-id="4e5b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e5b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e5b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e5b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e5b5-107">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="4e5b5-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="4e5b5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e5b5-108">Properties</span></span>
|<span data-ttu-id="4e5b5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e5b5-109">Property</span></span>|<span data-ttu-id="4e5b5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4e5b5-110">Type</span></span>|<span data-ttu-id="4e5b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4e5b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e5b5-112">name</span><span class="sxs-lookup"><span data-stu-id="4e5b5-112">name</span></span>|<span data-ttu-id="4e5b5-113">String</span><span class="sxs-lookup"><span data-stu-id="4e5b5-113">String</span></span>|<span data-ttu-id="4e5b5-114">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="4e5b5-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="4e5b5-115">обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="4e5b5-115">objectIdentifier</span></span>|<span data-ttu-id="4e5b5-116">String</span><span class="sxs-lookup"><span data-stu-id="4e5b5-116">String</span></span>|<span data-ttu-id="4e5b5-117">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="4e5b5-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e5b5-118">Связи</span><span class="sxs-lookup"><span data-stu-id="4e5b5-118">Relationships</span></span>
<span data-ttu-id="4e5b5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="4e5b5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e5b5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e5b5-120">JSON Representation</span></span>
<span data-ttu-id="4e5b5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-121">Here is a JSON representation of the resource.</span></span>
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





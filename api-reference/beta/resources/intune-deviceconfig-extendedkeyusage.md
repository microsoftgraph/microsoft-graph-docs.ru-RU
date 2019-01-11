---
title: Тип ресурса extendedKeyUsage
description: Настраиваемые определения расширенное использование ключа
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f1fd159a9b9fdb621a1e52bd080c005c8b93129c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840980"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="1bd8a-103">Тип ресурса extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="1bd8a-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="1bd8a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1bd8a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bd8a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bd8a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1bd8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bd8a-107">Настраиваемые определения расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="1bd8a-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="1bd8a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bd8a-108">Properties</span></span>
|<span data-ttu-id="1bd8a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bd8a-109">Property</span></span>|<span data-ttu-id="1bd8a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1bd8a-110">Type</span></span>|<span data-ttu-id="1bd8a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1bd8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd8a-112">name</span><span class="sxs-lookup"><span data-stu-id="1bd8a-112">name</span></span>|<span data-ttu-id="1bd8a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1bd8a-113">String</span></span>|<span data-ttu-id="1bd8a-114">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="1bd8a-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="1bd8a-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="1bd8a-115">objectIdentifier</span></span>|<span data-ttu-id="1bd8a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="1bd8a-116">String</span></span>|<span data-ttu-id="1bd8a-117">Расширенного использования ключа идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="1bd8a-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bd8a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1bd8a-118">Relationships</span></span>
<span data-ttu-id="1bd8a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1bd8a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1bd8a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bd8a-120">JSON Representation</span></span>
<span data-ttu-id="1bd8a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bd8a-121">Here is a JSON representation of the resource.</span></span>
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






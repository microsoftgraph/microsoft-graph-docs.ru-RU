---
title: Тип ресурса extendedKeyUsage
description: Настраиваемые определения расширенное использование ключа
author: tfitzmac
ms.openlocfilehash: 2b6155a0fbb234cb0b2081a8a4a226a8d218dbc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337291"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="2d12a-103">Тип ресурса extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="2d12a-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="2d12a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2d12a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d12a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d12a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d12a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d12a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d12a-107">Настраиваемые определения расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="2d12a-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="2d12a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d12a-108">Properties</span></span>
|<span data-ttu-id="2d12a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d12a-109">Property</span></span>|<span data-ttu-id="2d12a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2d12a-110">Type</span></span>|<span data-ttu-id="2d12a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2d12a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d12a-112">name</span><span class="sxs-lookup"><span data-stu-id="2d12a-112">name</span></span>|<span data-ttu-id="2d12a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2d12a-113">String</span></span>|<span data-ttu-id="2d12a-114">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="2d12a-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="2d12a-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="2d12a-115">objectIdentifier</span></span>|<span data-ttu-id="2d12a-116">String.</span><span class="sxs-lookup"><span data-stu-id="2d12a-116">String</span></span>|<span data-ttu-id="2d12a-117">Расширенного использования ключа идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="2d12a-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d12a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2d12a-118">Relationships</span></span>
<span data-ttu-id="2d12a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2d12a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d12a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d12a-120">JSON Representation</span></span>
<span data-ttu-id="2d12a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d12a-121">Here is a JSON representation of the resource.</span></span>
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






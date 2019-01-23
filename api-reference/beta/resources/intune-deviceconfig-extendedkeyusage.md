---
title: Тип ресурса extendedKeyUsage
description: Настраиваемые определения расширенное использование ключа
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ed825f44923d3fe86cc410397747b50a1f2c681
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425969"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="6c164-103">Тип ресурса extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="6c164-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="6c164-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6c164-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c164-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c164-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c164-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c164-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c164-107">Настраиваемые определения расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="6c164-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="6c164-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c164-108">Properties</span></span>
|<span data-ttu-id="6c164-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c164-109">Property</span></span>|<span data-ttu-id="6c164-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6c164-110">Type</span></span>|<span data-ttu-id="6c164-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6c164-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c164-112">name</span><span class="sxs-lookup"><span data-stu-id="6c164-112">name</span></span>|<span data-ttu-id="6c164-113">String</span><span class="sxs-lookup"><span data-stu-id="6c164-113">String</span></span>|<span data-ttu-id="6c164-114">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="6c164-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="6c164-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="6c164-115">objectIdentifier</span></span>|<span data-ttu-id="6c164-116">String</span><span class="sxs-lookup"><span data-stu-id="6c164-116">String</span></span>|<span data-ttu-id="6c164-117">Расширенного использования ключа идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="6c164-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c164-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="6c164-118">Relationships</span></span>
<span data-ttu-id="6c164-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6c164-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c164-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c164-120">JSON Representation</span></span>
<span data-ttu-id="6c164-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c164-121">Here is a JSON representation of the resource.</span></span>
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





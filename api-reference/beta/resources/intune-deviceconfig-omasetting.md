---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59a0d38eca6e448457d208eb9981c9de51031489
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273188"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="dd35c-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="dd35c-103">omaSetting resource type</span></span>

<span data-ttu-id="dd35c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd35c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd35c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd35c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd35c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd35c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd35c-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="dd35c-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="dd35c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd35c-108">Properties</span></span>
|<span data-ttu-id="dd35c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd35c-109">Property</span></span>|<span data-ttu-id="dd35c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dd35c-110">Type</span></span>|<span data-ttu-id="dd35c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dd35c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd35c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="dd35c-112">displayName</span></span>|<span data-ttu-id="dd35c-113">String</span><span class="sxs-lookup"><span data-stu-id="dd35c-113">String</span></span>|<span data-ttu-id="dd35c-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="dd35c-114">Display Name.</span></span>|
|<span data-ttu-id="dd35c-115">description</span><span class="sxs-lookup"><span data-stu-id="dd35c-115">description</span></span>|<span data-ttu-id="dd35c-116">String</span><span class="sxs-lookup"><span data-stu-id="dd35c-116">String</span></span>|<span data-ttu-id="dd35c-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="dd35c-117">Description.</span></span>|
|<span data-ttu-id="dd35c-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="dd35c-118">omaUri</span></span>|<span data-ttu-id="dd35c-119">String</span><span class="sxs-lookup"><span data-stu-id="dd35c-119">String</span></span>|<span data-ttu-id="dd35c-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="dd35c-120">OMA.</span></span>|
|<span data-ttu-id="dd35c-121">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="dd35c-121">isEncrypted</span></span>|<span data-ttu-id="dd35c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd35c-122">Boolean</span></span>|<span data-ttu-id="dd35c-123">Указывает, зашифровано ли поле "значение".</span><span class="sxs-lookup"><span data-stu-id="dd35c-123">Indicates whether the value field is encrypted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd35c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="dd35c-124">Relationships</span></span>
<span data-ttu-id="dd35c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="dd35c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd35c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd35c-126">JSON Representation</span></span>
<span data-ttu-id="dd35c-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd35c-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "isEncrypted": true
}
```





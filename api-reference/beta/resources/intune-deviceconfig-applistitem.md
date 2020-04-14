---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a34b8dcfbf3912d5b2a816ddfce6af49596b869
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469961"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="4f615-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="4f615-103">appListItem resource type</span></span>

<span data-ttu-id="4f615-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f615-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f615-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f615-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f615-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f615-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f615-107">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="4f615-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="4f615-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f615-108">Properties</span></span>
|<span data-ttu-id="4f615-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f615-109">Property</span></span>|<span data-ttu-id="4f615-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4f615-110">Type</span></span>|<span data-ttu-id="4f615-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4f615-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f615-112">name</span><span class="sxs-lookup"><span data-stu-id="4f615-112">name</span></span>|<span data-ttu-id="4f615-113">Строка</span><span class="sxs-lookup"><span data-stu-id="4f615-113">String</span></span>|<span data-ttu-id="4f615-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="4f615-114">The application name</span></span>|
|<span data-ttu-id="4f615-115">publisher</span><span class="sxs-lookup"><span data-stu-id="4f615-115">publisher</span></span>|<span data-ttu-id="4f615-116">String</span><span class="sxs-lookup"><span data-stu-id="4f615-116">String</span></span>|<span data-ttu-id="4f615-117">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="4f615-117">The publisher of the application</span></span>|
|<span data-ttu-id="4f615-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4f615-118">appStoreUrl</span></span>|<span data-ttu-id="4f615-119">String</span><span class="sxs-lookup"><span data-stu-id="4f615-119">String</span></span>|<span data-ttu-id="4f615-120">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="4f615-120">The Store URL of the application</span></span>|
|<span data-ttu-id="4f615-121">appId</span><span class="sxs-lookup"><span data-stu-id="4f615-121">appId</span></span>|<span data-ttu-id="4f615-122">String</span><span class="sxs-lookup"><span data-stu-id="4f615-122">String</span></span>|<span data-ttu-id="4f615-123">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="4f615-123">The bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f615-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="4f615-124">Relationships</span></span>
<span data-ttu-id="4f615-125">Нет</span><span class="sxs-lookup"><span data-stu-id="4f615-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f615-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f615-126">JSON Representation</span></span>
<span data-ttu-id="4f615-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f615-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
ms.openlocfilehash: c9b39b5fdee8bb503ef66f729a6ee478581a6391
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025021"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="dfbe4-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="dfbe4-103">appListItem resource type</span></span>

> <span data-ttu-id="dfbe4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dfbe4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfbe4-105">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="dfbe4-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="dfbe4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfbe4-106">Properties</span></span>
|<span data-ttu-id="dfbe4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfbe4-107">Property</span></span>|<span data-ttu-id="dfbe4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dfbe4-108">Type</span></span>|<span data-ttu-id="dfbe4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dfbe4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfbe4-110">name</span><span class="sxs-lookup"><span data-stu-id="dfbe4-110">name</span></span>|<span data-ttu-id="dfbe4-111">String</span><span class="sxs-lookup"><span data-stu-id="dfbe4-111">String</span></span>|<span data-ttu-id="dfbe4-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="dfbe4-112">The application name</span></span>|
|<span data-ttu-id="dfbe4-113">publisher</span><span class="sxs-lookup"><span data-stu-id="dfbe4-113">publisher</span></span>|<span data-ttu-id="dfbe4-114">String</span><span class="sxs-lookup"><span data-stu-id="dfbe4-114">String</span></span>|<span data-ttu-id="dfbe4-115">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="dfbe4-115">The publisher of the application</span></span>|
|<span data-ttu-id="dfbe4-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="dfbe4-116">appStoreUrl</span></span>|<span data-ttu-id="dfbe4-117">String</span><span class="sxs-lookup"><span data-stu-id="dfbe4-117">String</span></span>|<span data-ttu-id="dfbe4-118">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="dfbe4-118">The Store URL of the application</span></span>|
|<span data-ttu-id="dfbe4-119">appId</span><span class="sxs-lookup"><span data-stu-id="dfbe4-119">appId</span></span>|<span data-ttu-id="dfbe4-120">String</span><span class="sxs-lookup"><span data-stu-id="dfbe4-120">String</span></span>|<span data-ttu-id="dfbe4-121">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="dfbe4-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfbe4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="dfbe4-122">Relationships</span></span>
<span data-ttu-id="dfbe4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="dfbe4-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfbe4-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfbe4-124">JSON Representation</span></span>
<span data-ttu-id="dfbe4-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfbe4-125">Here is a JSON representation of the resource.</span></span>
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




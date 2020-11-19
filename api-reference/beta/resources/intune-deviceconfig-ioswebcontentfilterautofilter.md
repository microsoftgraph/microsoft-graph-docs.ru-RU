---
title: Тип ресурса Иосвебконтентфилтераутофилтер
description: Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c1c294ae84da91c6c61bb195fb79ea25c33134ac
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215872"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="29593-104">Тип ресурса Иосвебконтентфилтераутофилтер</span><span class="sxs-lookup"><span data-stu-id="29593-104">iosWebContentFilterAutoFilter resource type</span></span>

<span data-ttu-id="29593-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29593-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29593-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29593-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29593-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29593-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29593-108">Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="29593-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="29593-109">При создании без значений свойств устройство iOS включит автоматический фильтр независимо.</span><span class="sxs-lookup"><span data-stu-id="29593-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="29593-110">Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="29593-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29593-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="29593-111">Properties</span></span>
|<span data-ttu-id="29593-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="29593-112">Property</span></span>|<span data-ttu-id="29593-113">Тип</span><span class="sxs-lookup"><span data-stu-id="29593-113">Type</span></span>|<span data-ttu-id="29593-114">Описание</span><span class="sxs-lookup"><span data-stu-id="29593-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29593-115">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="29593-115">allowedUrls</span></span>|<span data-ttu-id="29593-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="29593-116">String collection</span></span>|<span data-ttu-id="29593-117">Дополнительные URL-адреса, разрешенные для Access</span><span class="sxs-lookup"><span data-stu-id="29593-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="29593-118">блоккедурлс</span><span class="sxs-lookup"><span data-stu-id="29593-118">blockedUrls</span></span>|<span data-ttu-id="29593-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="29593-119">String collection</span></span>|<span data-ttu-id="29593-120">Дополнительные URL-адреса, заблокированные для Access</span><span class="sxs-lookup"><span data-stu-id="29593-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="29593-121">Связи</span><span class="sxs-lookup"><span data-stu-id="29593-121">Relationships</span></span>
<span data-ttu-id="29593-122">Нет</span><span class="sxs-lookup"><span data-stu-id="29593-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29593-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29593-123">JSON Representation</span></span>
<span data-ttu-id="29593-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29593-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```





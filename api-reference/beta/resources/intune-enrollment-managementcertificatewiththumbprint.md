---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b849da155f0431ba5fd505e04fac23e077753159
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49197879"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="020fe-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="020fe-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="020fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="020fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="020fe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="020fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="020fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="020fe-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="020fe-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="020fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="020fe-108">Properties</span></span>
|<span data-ttu-id="020fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="020fe-109">Property</span></span>|<span data-ttu-id="020fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="020fe-110">Type</span></span>|<span data-ttu-id="020fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="020fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="020fe-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="020fe-112">thumbprint</span></span>|<span data-ttu-id="020fe-113">String</span><span class="sxs-lookup"><span data-stu-id="020fe-113">String</span></span>|<span data-ttu-id="020fe-114">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="020fe-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="020fe-115">certificate</span><span class="sxs-lookup"><span data-stu-id="020fe-115">certificate</span></span>|<span data-ttu-id="020fe-116">String</span><span class="sxs-lookup"><span data-stu-id="020fe-116">String</span></span>|<span data-ttu-id="020fe-117">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="020fe-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="020fe-118">Связи</span><span class="sxs-lookup"><span data-stu-id="020fe-118">Relationships</span></span>
<span data-ttu-id="020fe-119">Нет</span><span class="sxs-lookup"><span data-stu-id="020fe-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="020fe-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="020fe-120">JSON Representation</span></span>
<span data-ttu-id="020fe-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="020fe-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```





---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa78c594179edcd5a1cf4bc1b6e331d95155fc4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079923"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="de75b-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="de75b-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="de75b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de75b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de75b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de75b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de75b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de75b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de75b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de75b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="de75b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="de75b-108">Properties</span></span>
|<span data-ttu-id="de75b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="de75b-109">Property</span></span>|<span data-ttu-id="de75b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="de75b-110">Type</span></span>|<span data-ttu-id="de75b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de75b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de75b-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="de75b-112">thumbprint</span></span>|<span data-ttu-id="de75b-113">String</span><span class="sxs-lookup"><span data-stu-id="de75b-113">String</span></span>|<span data-ttu-id="de75b-114">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="de75b-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="de75b-115">certificate</span><span class="sxs-lookup"><span data-stu-id="de75b-115">certificate</span></span>|<span data-ttu-id="de75b-116">String</span><span class="sxs-lookup"><span data-stu-id="de75b-116">String</span></span>|<span data-ttu-id="de75b-117">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="de75b-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="de75b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="de75b-118">Relationships</span></span>
<span data-ttu-id="de75b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="de75b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de75b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de75b-120">JSON Representation</span></span>
<span data-ttu-id="de75b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de75b-121">Here is a JSON representation of the resource.</span></span>
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







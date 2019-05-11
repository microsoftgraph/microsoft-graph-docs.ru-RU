---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: affabd87c08d3e40ade9086fc7a0ad44f57facea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941494"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="46ec1-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="46ec1-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="46ec1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ec1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46ec1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46ec1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46ec1-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="46ec1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="46ec1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="46ec1-107">Properties</span></span>
|<span data-ttu-id="46ec1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="46ec1-108">Property</span></span>|<span data-ttu-id="46ec1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="46ec1-109">Type</span></span>|<span data-ttu-id="46ec1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="46ec1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46ec1-111">отпечаток</span><span class="sxs-lookup"><span data-stu-id="46ec1-111">thumbprint</span></span>|<span data-ttu-id="46ec1-112">Строка</span><span class="sxs-lookup"><span data-stu-id="46ec1-112">String</span></span>|<span data-ttu-id="46ec1-113">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="46ec1-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="46ec1-114">certificate</span><span class="sxs-lookup"><span data-stu-id="46ec1-114">certificate</span></span>|<span data-ttu-id="46ec1-115">String</span><span class="sxs-lookup"><span data-stu-id="46ec1-115">String</span></span>|<span data-ttu-id="46ec1-116">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="46ec1-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="46ec1-117">Связи</span><span class="sxs-lookup"><span data-stu-id="46ec1-117">Relationships</span></span>
<span data-ttu-id="46ec1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="46ec1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46ec1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46ec1-119">JSON Representation</span></span>
<span data-ttu-id="46ec1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46ec1-120">Here is a JSON representation of the resource.</span></span>
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





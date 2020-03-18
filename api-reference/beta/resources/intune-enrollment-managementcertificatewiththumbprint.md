---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9fad4b5e129b81d4fba37c19f25d20b59e16236
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783419"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="d3dd5-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="d3dd5-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="d3dd5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3dd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3dd5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3dd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3dd5-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3dd5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d3dd5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3dd5-107">Properties</span></span>
|<span data-ttu-id="d3dd5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3dd5-108">Property</span></span>|<span data-ttu-id="d3dd5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d3dd5-109">Type</span></span>|<span data-ttu-id="d3dd5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3dd5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3dd5-111">отпечаток</span><span class="sxs-lookup"><span data-stu-id="d3dd5-111">thumbprint</span></span>|<span data-ttu-id="d3dd5-112">String</span><span class="sxs-lookup"><span data-stu-id="d3dd5-112">String</span></span>|<span data-ttu-id="d3dd5-113">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="d3dd5-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="d3dd5-114">certificate</span><span class="sxs-lookup"><span data-stu-id="d3dd5-114">certificate</span></span>|<span data-ttu-id="d3dd5-115">String</span><span class="sxs-lookup"><span data-stu-id="d3dd5-115">String</span></span>|<span data-ttu-id="d3dd5-116">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="d3dd5-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3dd5-117">Связи</span><span class="sxs-lookup"><span data-stu-id="d3dd5-117">Relationships</span></span>
<span data-ttu-id="d3dd5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d3dd5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3dd5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3dd5-119">JSON Representation</span></span>
<span data-ttu-id="d3dd5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3dd5-120">Here is a JSON representation of the resource.</span></span>
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




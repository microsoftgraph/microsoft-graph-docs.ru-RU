---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58b45f092848be7198141a34a443471426be273b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773709"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="a1243-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="a1243-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="a1243-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1243-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1243-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1243-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a1243-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a1243-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1243-107">Properties</span></span>
|<span data-ttu-id="a1243-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1243-108">Property</span></span>|<span data-ttu-id="a1243-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a1243-109">Type</span></span>|<span data-ttu-id="a1243-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a1243-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1243-111">отпечаток</span><span class="sxs-lookup"><span data-stu-id="a1243-111">thumbprint</span></span>|<span data-ttu-id="a1243-112">String</span><span class="sxs-lookup"><span data-stu-id="a1243-112">String</span></span>|<span data-ttu-id="a1243-113">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="a1243-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="a1243-114">certificate</span><span class="sxs-lookup"><span data-stu-id="a1243-114">certificate</span></span>|<span data-ttu-id="a1243-115">String</span><span class="sxs-lookup"><span data-stu-id="a1243-115">String</span></span>|<span data-ttu-id="a1243-116">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="a1243-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1243-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="a1243-117">Relationships</span></span>
<span data-ttu-id="a1243-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a1243-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1243-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1243-119">JSON Representation</span></span>
<span data-ttu-id="a1243-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1243-120">Here is a JSON representation of the resource.</span></span>
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






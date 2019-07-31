---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 830c4ef0f6368dc573a50232fcc9beed36750d3e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999005"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="bbf0d-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="bbf0d-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="bbf0d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbf0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbf0d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbf0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbf0d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bbf0d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bbf0d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbf0d-107">Properties</span></span>
|<span data-ttu-id="bbf0d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbf0d-108">Property</span></span>|<span data-ttu-id="bbf0d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bbf0d-109">Type</span></span>|<span data-ttu-id="bbf0d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bbf0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbf0d-111">отпечаток</span><span class="sxs-lookup"><span data-stu-id="bbf0d-111">thumbprint</span></span>|<span data-ttu-id="bbf0d-112">String</span><span class="sxs-lookup"><span data-stu-id="bbf0d-112">String</span></span>|<span data-ttu-id="bbf0d-113">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="bbf0d-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="bbf0d-114">certificate</span><span class="sxs-lookup"><span data-stu-id="bbf0d-114">certificate</span></span>|<span data-ttu-id="bbf0d-115">String</span><span class="sxs-lookup"><span data-stu-id="bbf0d-115">String</span></span>|<span data-ttu-id="bbf0d-116">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="bbf0d-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbf0d-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="bbf0d-117">Relationships</span></span>
<span data-ttu-id="bbf0d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bbf0d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbf0d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbf0d-119">JSON Representation</span></span>
<span data-ttu-id="bbf0d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbf0d-120">Here is a JSON representation of the resource.</span></span>
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






---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 45a8544f9c032c386f99caa2f8d174d495673c29
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460724"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="3c84c-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="3c84c-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="3c84c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c84c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c84c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c84c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c84c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c84c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c84c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3c84c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3c84c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c84c-108">Properties</span></span>
|<span data-ttu-id="3c84c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c84c-109">Property</span></span>|<span data-ttu-id="3c84c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3c84c-110">Type</span></span>|<span data-ttu-id="3c84c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c84c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c84c-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="3c84c-112">thumbprint</span></span>|<span data-ttu-id="3c84c-113">String</span><span class="sxs-lookup"><span data-stu-id="3c84c-113">String</span></span>|<span data-ttu-id="3c84c-114">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="3c84c-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="3c84c-115">certificate</span><span class="sxs-lookup"><span data-stu-id="3c84c-115">certificate</span></span>|<span data-ttu-id="3c84c-116">String</span><span class="sxs-lookup"><span data-stu-id="3c84c-116">String</span></span>|<span data-ttu-id="3c84c-117">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="3c84c-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c84c-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="3c84c-118">Relationships</span></span>
<span data-ttu-id="3c84c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3c84c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c84c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c84c-120">JSON Representation</span></span>
<span data-ttu-id="3c84c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c84c-121">Here is a JSON representation of the resource.</span></span>
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




---
title: Тип ресурса Андроиденроллменткомпаникоде
description: Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ccc8cd1c1753c844ac5a71f9248f8189dad1e0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367101"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="2ba44-103">Тип ресурса Андроиденроллменткомпаникоде</span><span class="sxs-lookup"><span data-stu-id="2ba44-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="2ba44-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ba44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ba44-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ba44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ba44-106">Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода</span><span class="sxs-lookup"><span data-stu-id="2ba44-106">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="2ba44-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ba44-107">Properties</span></span>
|<span data-ttu-id="2ba44-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ba44-108">Property</span></span>|<span data-ttu-id="2ba44-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ba44-109">Type</span></span>|<span data-ttu-id="2ba44-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba44-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba44-111">енроллменттокен</span><span class="sxs-lookup"><span data-stu-id="2ba44-111">enrollmentToken</span></span>|<span data-ttu-id="2ba44-112">String</span><span class="sxs-lookup"><span data-stu-id="2ba44-112">String</span></span>|<span data-ttu-id="2ba44-113">Маркер регистрации, используемый пользователем для регистрации своего устройства.</span><span class="sxs-lookup"><span data-stu-id="2ba44-113">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="2ba44-114">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="2ba44-114">qrCodeContent</span></span>|<span data-ttu-id="2ba44-115">String</span><span class="sxs-lookup"><span data-stu-id="2ba44-115">String</span></span>|<span data-ttu-id="2ba44-116">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="2ba44-116">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="2ba44-117">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="2ba44-117">qrCodeImage</span></span>|[<span data-ttu-id="2ba44-118">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2ba44-118">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2ba44-119">Созданный QR код для маркера.</span><span class="sxs-lookup"><span data-stu-id="2ba44-119">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ba44-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ba44-120">Relationships</span></span>
<span data-ttu-id="2ba44-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2ba44-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ba44-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ba44-122">JSON Representation</span></span>
<span data-ttu-id="2ba44-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ba44-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




---
title: Тип ресурса Андроиденроллменткомпаникоде
description: Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffb11de69dfe1f2a6a82e59024518b4d68676844
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736340"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="f3088-103">Тип ресурса Андроиденроллменткомпаникоде</span><span class="sxs-lookup"><span data-stu-id="f3088-103">androidEnrollmentCompanyCode resource type</span></span>

<span data-ttu-id="f3088-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3088-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3088-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3088-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3088-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3088-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3088-107">Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода</span><span class="sxs-lookup"><span data-stu-id="f3088-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="f3088-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3088-108">Properties</span></span>
|<span data-ttu-id="f3088-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3088-109">Property</span></span>|<span data-ttu-id="f3088-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f3088-110">Type</span></span>|<span data-ttu-id="f3088-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f3088-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3088-112">енроллменттокен</span><span class="sxs-lookup"><span data-stu-id="f3088-112">enrollmentToken</span></span>|<span data-ttu-id="f3088-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f3088-113">String</span></span>|<span data-ttu-id="f3088-114">Маркер регистрации, используемый пользователем для регистрации своего устройства.</span><span class="sxs-lookup"><span data-stu-id="f3088-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="f3088-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="f3088-115">qrCodeContent</span></span>|<span data-ttu-id="f3088-116">String</span><span class="sxs-lookup"><span data-stu-id="f3088-116">String</span></span>|<span data-ttu-id="f3088-117">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="f3088-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="f3088-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="f3088-118">qrCodeImage</span></span>|[<span data-ttu-id="f3088-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3088-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3088-120">Созданный QR код для маркера.</span><span class="sxs-lookup"><span data-stu-id="f3088-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3088-121">Связи</span><span class="sxs-lookup"><span data-stu-id="f3088-121">Relationships</span></span>
<span data-ttu-id="f3088-122">Нет</span><span class="sxs-lookup"><span data-stu-id="f3088-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3088-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3088-123">JSON Representation</span></span>
<span data-ttu-id="f3088-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3088-124">Here is a JSON representation of the resource.</span></span>
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






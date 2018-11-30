---
title: Тип ресурса bitLockerRecoveryOptions
description: Варианты восстановления BitLocker.
ms.openlocfilehash: 46af5b52d8305932d0d67ef57d6a1f356182a469
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076870"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="0fc45-103">Тип ресурса bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="0fc45-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="0fc45-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0fc45-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fc45-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fc45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fc45-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0fc45-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fc45-107">Варианты восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="0fc45-107">BitLocker Recovery Options.</span></span>
## <a name="properties"></a><span data-ttu-id="0fc45-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fc45-108">Properties</span></span>
|<span data-ttu-id="0fc45-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fc45-109">Property</span></span>|<span data-ttu-id="0fc45-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0fc45-110">Type</span></span>|<span data-ttu-id="0fc45-111">Description</span><span class="sxs-lookup"><span data-stu-id="0fc45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc45-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="0fc45-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="0fc45-113">Логический</span><span class="sxs-lookup"><span data-stu-id="0fc45-113">Boolean</span></span>|<span data-ttu-id="0fc45-114">Указывает, следует ли блокировать агентом восстановления данных на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="0fc45-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="0fc45-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="0fc45-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="0fc45-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="0fc45-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="0fc45-117">Указывает ли пользователи могут или должны создавать пароль восстановления из 48 цифр основных или системный диск.</span><span class="sxs-lookup"><span data-stu-id="0fc45-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="0fc45-118">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="0fc45-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="0fc45-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="0fc45-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="0fc45-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="0fc45-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="0fc45-121">Указывает ли пользователям разрешено или необходимо создание ключа восстановления 256-разрядный основных или системный диск.</span><span class="sxs-lookup"><span data-stu-id="0fc45-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="0fc45-122">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="0fc45-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="0fc45-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="0fc45-123">hideRecoveryOptions</span></span>|<span data-ttu-id="0fc45-124">Логический</span><span class="sxs-lookup"><span data-stu-id="0fc45-124">Boolean</span></span>|<span data-ttu-id="0fc45-125">Указывает ли разрешать отображение параметры восстановления в мастер установки BitLocker основных или системный диск.</span><span class="sxs-lookup"><span data-stu-id="0fc45-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="0fc45-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="0fc45-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="0fc45-127">Логический</span><span class="sxs-lookup"><span data-stu-id="0fc45-127">Boolean</span></span>|<span data-ttu-id="0fc45-128">Указывает, следует ли разрешить сведения о восстановлении BitLocker для хранения в Доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0fc45-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="0fc45-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="0fc45-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="0fc45-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="0fc45-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="0fc45-131">Настройте, какие части сведения о восстановлении BitLocker хранятся в Доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0fc45-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="0fc45-132">Возможные значения: `passwordAndKey`, `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="0fc45-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="0fc45-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="0fc45-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="0fc45-134">Логический</span><span class="sxs-lookup"><span data-stu-id="0fc45-134">Boolean</span></span>|<span data-ttu-id="0fc45-135">Указывает, следует ли включить BitLocker до восстановления данные хранятся в Доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0fc45-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fc45-136">Связи</span><span class="sxs-lookup"><span data-stu-id="0fc45-136">Relationships</span></span>
<span data-ttu-id="0fc45-137">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc45-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0fc45-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0fc45-138">JSON Representation</span></span>
<span data-ttu-id="0fc45-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fc45-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```






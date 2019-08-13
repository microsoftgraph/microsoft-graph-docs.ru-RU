---
title: Тип ресурса Bitlockersystemdrivepolicy.
description: Основные политики шифрования BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4ffeaca0d5ee305690c05337eeb75787ece9641
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333767"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="2ee98-103">Тип ресурса Bitlockersystemdrivepolicy.</span><span class="sxs-lookup"><span data-stu-id="2ee98-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="2ee98-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ee98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ee98-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ee98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ee98-106">Основные политики шифрования BitLocker.</span><span class="sxs-lookup"><span data-stu-id="2ee98-106">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="2ee98-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ee98-107">Properties</span></span>
|<span data-ttu-id="2ee98-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ee98-108">Property</span></span>|<span data-ttu-id="2ee98-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ee98-109">Type</span></span>|<span data-ttu-id="2ee98-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ee98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ee98-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="2ee98-111">encryptionMethod</span></span>|[<span data-ttu-id="2ee98-112">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="2ee98-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="2ee98-113">Выберите метод шифрования для дисков операционной системы.</span><span class="sxs-lookup"><span data-stu-id="2ee98-113">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="2ee98-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="2ee98-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="2ee98-115">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="2ee98-115">startupAuthenticationRequired</span></span>|<span data-ttu-id="2ee98-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ee98-116">Boolean</span></span>|<span data-ttu-id="2ee98-117">Требовать дополнительной проверки подлинности при запуске.</span><span class="sxs-lookup"><span data-stu-id="2ee98-117">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="2ee98-118">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="2ee98-118">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="2ee98-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ee98-119">Boolean</span></span>|<span data-ttu-id="2ee98-120">Указывает, следует ли разрешить BitLocker без совместимого доверенного платформенного модуля (требуется пароль или ключ запуска на USB флэш-накопителе).</span><span class="sxs-lookup"><span data-stu-id="2ee98-120">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="2ee98-121">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="2ee98-121">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="2ee98-122">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="2ee98-122">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="2ee98-123">Указывает, разрешена или не разрешена или необязательная Загрузка TPM.</span><span class="sxs-lookup"><span data-stu-id="2ee98-123">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="2ee98-124">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="2ee98-124">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="2ee98-125">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="2ee98-125">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="2ee98-126">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="2ee98-126">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="2ee98-127">Указывает, разрешен ли ПИН-код для запуска TPM, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="2ee98-127">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="2ee98-128">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="2ee98-128">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="2ee98-129">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="2ee98-129">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="2ee98-130">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="2ee98-130">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="2ee98-131">Указывает, разрешен ли ключ запуска TPM, обязательный, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="2ee98-131">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="2ee98-132">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="2ee98-132">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="2ee98-133">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="2ee98-133">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="2ee98-134">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="2ee98-134">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="2ee98-135">Указывает, разрешены ли ключ и ключ ПИН-кода для запуска TPM, а какие — обязательные или запрещенные.</span><span class="sxs-lookup"><span data-stu-id="2ee98-135">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="2ee98-136">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="2ee98-136">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="2ee98-137">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="2ee98-137">minimumPinLength</span></span>|<span data-ttu-id="2ee98-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2ee98-138">Int32</span></span>|<span data-ttu-id="2ee98-139">Указывает минимальную длину ПИН-кода для запуска.</span><span class="sxs-lookup"><span data-stu-id="2ee98-139">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="2ee98-140">Допустимые значения — от 4 до 20.</span><span class="sxs-lookup"><span data-stu-id="2ee98-140">Valid values 4 to 20</span></span>|
|<span data-ttu-id="2ee98-141">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="2ee98-141">recoveryOptions</span></span>|<span data-ttu-id="2ee98-142">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="2ee98-142">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="2ee98-143">Позволяет восстанавливать зашифрованные диски операционной системы BitLocker в отсутствие требуемых сведений о ключе запуска.</span><span class="sxs-lookup"><span data-stu-id="2ee98-143">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="2ee98-144">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="2ee98-144">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="2ee98-145">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="2ee98-145">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="2ee98-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ee98-146">Boolean</span></span>|<span data-ttu-id="2ee98-147">Включение сообщения о восстановлении перед загрузкой и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="2ee98-147">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="2ee98-148">Если Рекуирестартупаусентикатион имеет значение false, это значение не влияет.</span><span class="sxs-lookup"><span data-stu-id="2ee98-148">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="2ee98-149">пребутрековеримессаже</span><span class="sxs-lookup"><span data-stu-id="2ee98-149">prebootRecoveryMessage</span></span>|<span data-ttu-id="2ee98-150">String</span><span class="sxs-lookup"><span data-stu-id="2ee98-150">String</span></span>|<span data-ttu-id="2ee98-151">Определяет настраиваемое сообщение о восстановлении.</span><span class="sxs-lookup"><span data-stu-id="2ee98-151">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="2ee98-152">пребутрековерюрл</span><span class="sxs-lookup"><span data-stu-id="2ee98-152">prebootRecoveryUrl</span></span>|<span data-ttu-id="2ee98-153">String</span><span class="sxs-lookup"><span data-stu-id="2ee98-153">String</span></span>|<span data-ttu-id="2ee98-154">Определяет настраиваемый URL-адрес для восстановления.</span><span class="sxs-lookup"><span data-stu-id="2ee98-154">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ee98-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ee98-155">Relationships</span></span>
<span data-ttu-id="2ee98-156">Нет</span><span class="sxs-lookup"><span data-stu-id="2ee98-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ee98-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ee98-157">JSON Representation</span></span>
<span data-ttu-id="2ee98-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ee98-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```




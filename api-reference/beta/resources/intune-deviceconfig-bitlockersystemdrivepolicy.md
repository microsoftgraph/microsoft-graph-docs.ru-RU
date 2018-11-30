---
title: Тип ресурса bitLockerSystemDrivePolicy
description: Базовый политики шифрования BitLocker.
ms.openlocfilehash: 60388f020750ebd7f187b07777440b013ae5f02a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077248"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="b6ca3-103">Тип ресурса bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b6ca3-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="b6ca3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6ca3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6ca3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6ca3-107">Базовый политики шифрования BitLocker.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-107">BitLocker Encryption Base Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="b6ca3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6ca3-108">Properties</span></span>
|<span data-ttu-id="b6ca3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6ca3-109">Property</span></span>|<span data-ttu-id="b6ca3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b6ca3-110">Type</span></span>|<span data-ttu-id="b6ca3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6ca3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6ca3-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b6ca3-112">encryptionMethod</span></span>|[<span data-ttu-id="b6ca3-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b6ca3-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="b6ca3-114">Выберите метод шифрования для дисков операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="b6ca3-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="b6ca3-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="b6ca3-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="b6ca3-117">Логический</span><span class="sxs-lookup"><span data-stu-id="b6ca3-117">Boolean</span></span>|<span data-ttu-id="b6ca3-118">Требовать дополнительную проверку подлинности при запуске системы.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="b6ca3-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="b6ca3-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="b6ca3-120">Логический</span><span class="sxs-lookup"><span data-stu-id="b6ca3-120">Boolean</span></span>|<span data-ttu-id="b6ca3-121">Указывает, следует ли разрешить BitLocker без совместимого TPM (требуется пароль или ключ запуска на флэш-накопитель USB).</span><span class="sxs-lookup"><span data-stu-id="b6ca3-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="b6ca3-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="b6ca3-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="b6ca3-124">Указывает, является ли запуска TPM разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="b6ca3-125">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="b6ca3-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="b6ca3-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="b6ca3-128">Указывает, является ли ПИН-кода запуска TPM разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="b6ca3-129">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="b6ca3-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="b6ca3-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="b6ca3-132">Указывает, является ли ключ запуска TPM разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="b6ca3-133">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="b6ca3-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="b6ca3-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="b6ca3-136">Указывает, если прикрепление запуска TPM и ключ разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="b6ca3-137">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="b6ca3-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="b6ca3-138">minimumPinLength</span></span>|<span data-ttu-id="b6ca3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b6ca3-139">Int32</span></span>|<span data-ttu-id="b6ca3-140">Указывает минимальную длину ПИН-кодов запуска.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="b6ca3-141">Допустимые значения 4 до 20</span><span class="sxs-lookup"><span data-stu-id="b6ca3-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="b6ca3-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="b6ca3-142">recoveryOptions</span></span>|<span data-ttu-id="b6ca3-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="b6ca3-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="b6ca3-144">Разрешает Восстановление зашифрованного BitLocker дисков операционной системы в случае отсутствия данные ключа требуется запуска.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="b6ca3-145">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="b6ca3-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="b6ca3-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="b6ca3-147">Логический</span><span class="sxs-lookup"><span data-stu-id="b6ca3-147">Boolean</span></span>|<span data-ttu-id="b6ca3-148">Включение восстановления до загрузки сообщение и URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="b6ca3-149">Если requireStartupAuthentication имеет значение false, это значение не влияет на.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="b6ca3-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="b6ca3-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="b6ca3-151">String</span><span class="sxs-lookup"><span data-stu-id="b6ca3-151">String</span></span>|<span data-ttu-id="b6ca3-152">Определяет сообщение настраиваемого восстановления.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="b6ca3-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="b6ca3-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="b6ca3-154">String</span><span class="sxs-lookup"><span data-stu-id="b6ca3-154">String</span></span>|<span data-ttu-id="b6ca3-155">Определяет URL-адрес настраиваемого восстановления.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6ca3-156">Связи</span><span class="sxs-lookup"><span data-stu-id="b6ca3-156">Relationships</span></span>
<span data-ttu-id="b6ca3-157">Нет</span><span class="sxs-lookup"><span data-stu-id="b6ca3-157">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6ca3-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6ca3-158">JSON Representation</span></span>
<span data-ttu-id="b6ca3-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6ca3-159">Here is a JSON representation of the resource.</span></span>
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






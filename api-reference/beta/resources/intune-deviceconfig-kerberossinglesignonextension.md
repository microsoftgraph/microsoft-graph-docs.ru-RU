---
title: Тип ресурса Кербероссинглесигнонекстенсион
description: Представляет профиль расширения единого входа Kerberos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 709ec5f558a147534a69d70fe165edd1cbece671
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790449"
---
# <a name="kerberossinglesignonextension-resource-type"></a><span data-ttu-id="04e8a-103">Тип ресурса Кербероссинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="04e8a-103">kerberosSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="04e8a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04e8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04e8a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04e8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04e8a-106">Представляет профиль расширения единого входа Kerberos.</span><span class="sxs-lookup"><span data-stu-id="04e8a-106">Represents a Kerberos-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="04e8a-107">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="04e8a-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04e8a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="04e8a-108">Properties</span></span>
|<span data-ttu-id="04e8a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="04e8a-109">Property</span></span>|<span data-ttu-id="04e8a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="04e8a-110">Type</span></span>|<span data-ttu-id="04e8a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04e8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e8a-112">область</span><span class="sxs-lookup"><span data-stu-id="04e8a-112">realm</span></span>|<span data-ttu-id="04e8a-113">String</span><span class="sxs-lookup"><span data-stu-id="04e8a-113">String</span></span>|<span data-ttu-id="04e8a-114">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="04e8a-114">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="04e8a-115">домена</span><span class="sxs-lookup"><span data-stu-id="04e8a-115">domains</span></span>|<span data-ttu-id="04e8a-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04e8a-116">String collection</span></span>|<span data-ttu-id="04e8a-117">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="04e8a-117">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="04e8a-118">блоккаутоматиклогин</span><span class="sxs-lookup"><span data-stu-id="04e8a-118">blockAutomaticLogin</span></span>|<span data-ttu-id="04e8a-119">Логический</span><span class="sxs-lookup"><span data-stu-id="04e8a-119">Boolean</span></span>|<span data-ttu-id="04e8a-120">Включает или отключает использование цепочки ключей.</span><span class="sxs-lookup"><span data-stu-id="04e8a-120">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="04e8a-121">каченаме</span><span class="sxs-lookup"><span data-stu-id="04e8a-121">cacheName</span></span>|<span data-ttu-id="04e8a-122">String</span><span class="sxs-lookup"><span data-stu-id="04e8a-122">String</span></span>|<span data-ttu-id="04e8a-123">Получает или задает универсальное имя службы безопасности для кэша Kerberos, который будет использоваться для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="04e8a-123">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="04e8a-124">кредентиалбундлеидакцессконтроллист</span><span class="sxs-lookup"><span data-stu-id="04e8a-124">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="04e8a-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04e8a-125">String collection</span></span>|<span data-ttu-id="04e8a-126">Получает или задает список идентификаторов пакетов приложений, которым разрешен доступ к билету предоставления билетов Kerberos.</span><span class="sxs-lookup"><span data-stu-id="04e8a-126">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="04e8a-127">домаинреалмс</span><span class="sxs-lookup"><span data-stu-id="04e8a-127">domainRealms</span></span>|<span data-ttu-id="04e8a-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04e8a-128">String collection</span></span>|<span data-ttu-id="04e8a-129">Получает или задает список сфер для сопоставления пользовательских областей доменов.</span><span class="sxs-lookup"><span data-stu-id="04e8a-129">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="04e8a-130">В сфере учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="04e8a-130">Realms are case sensitive.</span></span>|
|<span data-ttu-id="04e8a-131">исдефаултреалм</span><span class="sxs-lookup"><span data-stu-id="04e8a-131">isDefaultRealm</span></span>|<span data-ttu-id="04e8a-132">Логический</span><span class="sxs-lookup"><span data-stu-id="04e8a-132">Boolean</span></span>|<span data-ttu-id="04e8a-133">Если задано значение true, область этого профиля будет выбрана по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="04e8a-133">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="04e8a-134">Необходимо, если настроено несколько профилей типа Kerberos.</span><span class="sxs-lookup"><span data-stu-id="04e8a-134">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="04e8a-135">пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="04e8a-135">passwordBlockModification</span></span>|<span data-ttu-id="04e8a-136">Логический</span><span class="sxs-lookup"><span data-stu-id="04e8a-136">Boolean</span></span>|<span data-ttu-id="04e8a-137">Включает или отключает смену паролей.</span><span class="sxs-lookup"><span data-stu-id="04e8a-137">Enables or disables password changes.</span></span>|
|<span data-ttu-id="04e8a-138">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="04e8a-138">passwordExpirationDays</span></span>|<span data-ttu-id="04e8a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="04e8a-139">Int32</span></span>|<span data-ttu-id="04e8a-140">Переопределяет срок действия пароля по умолчанию (в днях).</span><span class="sxs-lookup"><span data-stu-id="04e8a-140">Overrides the default password expiration in days.</span></span> <span data-ttu-id="04e8a-141">Для большинства доменов это значение вычисляется автоматически.</span><span class="sxs-lookup"><span data-stu-id="04e8a-141">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="04e8a-142">пассвордекспиратионнотификатиондайс</span><span class="sxs-lookup"><span data-stu-id="04e8a-142">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="04e8a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="04e8a-143">Int32</span></span>|<span data-ttu-id="04e8a-144">Получает или задает количество дней до тех пор, пока пользователь не будет уведомлен о сроке действия пароля (значение по умолчанию — 15).</span><span class="sxs-lookup"><span data-stu-id="04e8a-144">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="04e8a-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="04e8a-145">userPrincipalName</span></span>|<span data-ttu-id="04e8a-146">String</span><span class="sxs-lookup"><span data-stu-id="04e8a-146">String</span></span>|<span data-ttu-id="04e8a-147">Получает или задает имя участника, которое будет использоваться для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="04e8a-147">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="04e8a-148">Имя области не обязательно должно быть включено.</span><span class="sxs-lookup"><span data-stu-id="04e8a-148">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="04e8a-149">пассвордрекуиреактиведиректорикомплексити</span><span class="sxs-lookup"><span data-stu-id="04e8a-149">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="04e8a-150">Логический</span><span class="sxs-lookup"><span data-stu-id="04e8a-150">Boolean</span></span>|<span data-ttu-id="04e8a-151">Разрешает или запрещает, должны ли пароли отвечать требованиям сложности Active Directory.</span><span class="sxs-lookup"><span data-stu-id="04e8a-151">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="04e8a-152">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="04e8a-152">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="04e8a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="04e8a-153">Int32</span></span>|<span data-ttu-id="04e8a-154">Получает или задает количество предыдущих паролей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="04e8a-154">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="04e8a-155">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="04e8a-155">passwordMinimumLength</span></span>|<span data-ttu-id="04e8a-156">Int32</span><span class="sxs-lookup"><span data-stu-id="04e8a-156">Int32</span></span>|<span data-ttu-id="04e8a-157">Получает или задает минимальную длину пароля.</span><span class="sxs-lookup"><span data-stu-id="04e8a-157">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="04e8a-158">пассвордминимумажедайс</span><span class="sxs-lookup"><span data-stu-id="04e8a-158">passwordMinimumAgeDays</span></span>|<span data-ttu-id="04e8a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="04e8a-159">Int32</span></span>|<span data-ttu-id="04e8a-160">Получает или задает минимальное количество дней, пока пользователь не сможет сменить пароль еще раз.</span><span class="sxs-lookup"><span data-stu-id="04e8a-160">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="04e8a-161">пассвордрекуирементсдескриптион</span><span class="sxs-lookup"><span data-stu-id="04e8a-161">passwordRequirementsDescription</span></span>|<span data-ttu-id="04e8a-162">String</span><span class="sxs-lookup"><span data-stu-id="04e8a-162">String</span></span>|<span data-ttu-id="04e8a-163">Получает или задает описание требований к сложности пароля.</span><span class="sxs-lookup"><span data-stu-id="04e8a-163">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="04e8a-164">рекуиреусерпресенце</span><span class="sxs-lookup"><span data-stu-id="04e8a-164">requireUserPresence</span></span>|<span data-ttu-id="04e8a-165">Логический</span><span class="sxs-lookup"><span data-stu-id="04e8a-165">Boolean</span></span>|<span data-ttu-id="04e8a-166">Получает или задает значение, указывающее, требуется ли проверка подлинности с помощью идентификатора сенсорного экрана, идентификатора лица или секретного кода для доступа к записи цепочки ключей.</span><span class="sxs-lookup"><span data-stu-id="04e8a-166">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="04e8a-167">активедиректориситекоде</span><span class="sxs-lookup"><span data-stu-id="04e8a-167">activeDirectorySiteCode</span></span>|<span data-ttu-id="04e8a-168">String</span><span class="sxs-lookup"><span data-stu-id="04e8a-168">String</span></span>|<span data-ttu-id="04e8a-169">Получает или задает сайт Active Directory.</span><span class="sxs-lookup"><span data-stu-id="04e8a-169">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="04e8a-170">пассворденаблелокалсинк</span><span class="sxs-lookup"><span data-stu-id="04e8a-170">passwordEnableLocalSync</span></span>|<span data-ttu-id="04e8a-171">Логический</span><span class="sxs-lookup"><span data-stu-id="04e8a-171">Boolean</span></span>|<span data-ttu-id="04e8a-172">Включает или отключает синхронизацию паролей.</span><span class="sxs-lookup"><span data-stu-id="04e8a-172">Enables or disables password syncing.</span></span> <span data-ttu-id="04e8a-173">Это не повлияет на пользователей, выполнивших вход в систему с помощью учетной записи мобильного устройства в macOS.</span><span class="sxs-lookup"><span data-stu-id="04e8a-173">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="04e8a-174">блоккактиведиректориситеаутодисковери</span><span class="sxs-lookup"><span data-stu-id="04e8a-174">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="04e8a-175">Логический</span><span class="sxs-lookup"><span data-stu-id="04e8a-175">Boolean</span></span>|<span data-ttu-id="04e8a-176">Включает или отключает, может ли расширение Kerberos автоматически определять имя своего сайта.</span><span class="sxs-lookup"><span data-stu-id="04e8a-176">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|
|<span data-ttu-id="04e8a-177">пассвордчанжеурл</span><span class="sxs-lookup"><span data-stu-id="04e8a-177">passwordChangeUrl</span></span>|<span data-ttu-id="04e8a-178">String</span><span class="sxs-lookup"><span data-stu-id="04e8a-178">String</span></span>|<span data-ttu-id="04e8a-179">Получает или задает URL-адрес, на который будет отправляться пользователь при инициации смены пароля.</span><span class="sxs-lookup"><span data-stu-id="04e8a-179">Gets or sets the URL that the user will be sent to when they initiate a password change.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04e8a-180">Связи</span><span class="sxs-lookup"><span data-stu-id="04e8a-180">Relationships</span></span>
<span data-ttu-id="04e8a-181">Нет</span><span class="sxs-lookup"><span data-stu-id="04e8a-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04e8a-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04e8a-182">JSON Representation</span></span>
<span data-ttu-id="04e8a-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04e8a-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.kerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.kerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```




---
title: Тип ресурса Макоскербероссинглесигнонекстенсион
description: Представляет профиль расширения единого входа Kerberos для устройств macOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 44abc4972e078bc0aac6e6be9a30357bd97a8198
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447063"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a><span data-ttu-id="aa655-103">Тип ресурса Макоскербероссинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="aa655-103">macOSKerberosSingleSignOnExtension resource type</span></span>

<span data-ttu-id="aa655-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa655-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa655-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa655-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa655-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa655-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa655-107">Представляет профиль расширения единого входа Kerberos для устройств macOS.</span><span class="sxs-lookup"><span data-stu-id="aa655-107">Represents a Kerberos-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="aa655-108">Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="aa655-108">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa655-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa655-109">Properties</span></span>
|<span data-ttu-id="aa655-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa655-110">Property</span></span>|<span data-ttu-id="aa655-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aa655-111">Type</span></span>|<span data-ttu-id="aa655-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aa655-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa655-113">область</span><span class="sxs-lookup"><span data-stu-id="aa655-113">realm</span></span>|<span data-ttu-id="aa655-114">String</span><span class="sxs-lookup"><span data-stu-id="aa655-114">String</span></span>|<span data-ttu-id="aa655-115">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="aa655-115">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="aa655-116">домена</span><span class="sxs-lookup"><span data-stu-id="aa655-116">domains</span></span>|<span data-ttu-id="aa655-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aa655-117">String collection</span></span>|<span data-ttu-id="aa655-118">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="aa655-118">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="aa655-119">блоккаутоматиклогин</span><span class="sxs-lookup"><span data-stu-id="aa655-119">blockAutomaticLogin</span></span>|<span data-ttu-id="aa655-120">Логическое</span><span class="sxs-lookup"><span data-stu-id="aa655-120">Boolean</span></span>|<span data-ttu-id="aa655-121">Включает или отключает использование цепочки ключей.</span><span class="sxs-lookup"><span data-stu-id="aa655-121">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="aa655-122">каченаме</span><span class="sxs-lookup"><span data-stu-id="aa655-122">cacheName</span></span>|<span data-ttu-id="aa655-123">String</span><span class="sxs-lookup"><span data-stu-id="aa655-123">String</span></span>|<span data-ttu-id="aa655-124">Получает или задает универсальное имя службы безопасности для кэша Kerberos, который будет использоваться для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="aa655-124">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="aa655-125">кредентиалбундлеидакцессконтроллист</span><span class="sxs-lookup"><span data-stu-id="aa655-125">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="aa655-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aa655-126">String collection</span></span>|<span data-ttu-id="aa655-127">Получает или задает список идентификаторов пакетов приложений, которым разрешен доступ к билету предоставления билетов Kerberos.</span><span class="sxs-lookup"><span data-stu-id="aa655-127">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="aa655-128">домаинреалмс</span><span class="sxs-lookup"><span data-stu-id="aa655-128">domainRealms</span></span>|<span data-ttu-id="aa655-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aa655-129">String collection</span></span>|<span data-ttu-id="aa655-130">Получает или задает список сфер для сопоставления пользовательских областей доменов.</span><span class="sxs-lookup"><span data-stu-id="aa655-130">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="aa655-131">В сфере учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="aa655-131">Realms are case sensitive.</span></span>|
|<span data-ttu-id="aa655-132">исдефаултреалм</span><span class="sxs-lookup"><span data-stu-id="aa655-132">isDefaultRealm</span></span>|<span data-ttu-id="aa655-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="aa655-133">Boolean</span></span>|<span data-ttu-id="aa655-134">Если задано значение true, область этого профиля будет выбрана по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="aa655-134">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="aa655-135">Необходимо, если настроено несколько профилей типа Kerberos.</span><span class="sxs-lookup"><span data-stu-id="aa655-135">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="aa655-136">пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="aa655-136">passwordBlockModification</span></span>|<span data-ttu-id="aa655-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="aa655-137">Boolean</span></span>|<span data-ttu-id="aa655-138">Включает или отключает смену паролей.</span><span class="sxs-lookup"><span data-stu-id="aa655-138">Enables or disables password changes.</span></span>|
|<span data-ttu-id="aa655-139">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aa655-139">passwordExpirationDays</span></span>|<span data-ttu-id="aa655-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aa655-140">Int32</span></span>|<span data-ttu-id="aa655-141">Переопределяет срок действия пароля по умолчанию (в днях).</span><span class="sxs-lookup"><span data-stu-id="aa655-141">Overrides the default password expiration in days.</span></span> <span data-ttu-id="aa655-142">Для большинства доменов это значение вычисляется автоматически.</span><span class="sxs-lookup"><span data-stu-id="aa655-142">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="aa655-143">пассвордекспиратионнотификатиондайс</span><span class="sxs-lookup"><span data-stu-id="aa655-143">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="aa655-144">Int32</span><span class="sxs-lookup"><span data-stu-id="aa655-144">Int32</span></span>|<span data-ttu-id="aa655-145">Получает или задает количество дней до тех пор, пока пользователь не будет уведомлен о сроке действия пароля (значение по умолчанию — 15).</span><span class="sxs-lookup"><span data-stu-id="aa655-145">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="aa655-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa655-146">userPrincipalName</span></span>|<span data-ttu-id="aa655-147">String</span><span class="sxs-lookup"><span data-stu-id="aa655-147">String</span></span>|<span data-ttu-id="aa655-148">Получает или задает имя участника, которое будет использоваться для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="aa655-148">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="aa655-149">Имя области не обязательно должно быть включено.</span><span class="sxs-lookup"><span data-stu-id="aa655-149">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="aa655-150">пассвордрекуиреактиведиректорикомплексити</span><span class="sxs-lookup"><span data-stu-id="aa655-150">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="aa655-151">Логическое</span><span class="sxs-lookup"><span data-stu-id="aa655-151">Boolean</span></span>|<span data-ttu-id="aa655-152">Разрешает или запрещает, должны ли пароли отвечать требованиям сложности Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa655-152">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="aa655-153">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aa655-153">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aa655-154">Int32</span><span class="sxs-lookup"><span data-stu-id="aa655-154">Int32</span></span>|<span data-ttu-id="aa655-155">Получает или задает количество предыдущих паролей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="aa655-155">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="aa655-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aa655-156">passwordMinimumLength</span></span>|<span data-ttu-id="aa655-157">Int32</span><span class="sxs-lookup"><span data-stu-id="aa655-157">Int32</span></span>|<span data-ttu-id="aa655-158">Получает или задает минимальную длину пароля.</span><span class="sxs-lookup"><span data-stu-id="aa655-158">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="aa655-159">пассвордминимумажедайс</span><span class="sxs-lookup"><span data-stu-id="aa655-159">passwordMinimumAgeDays</span></span>|<span data-ttu-id="aa655-160">Int32</span><span class="sxs-lookup"><span data-stu-id="aa655-160">Int32</span></span>|<span data-ttu-id="aa655-161">Получает или задает минимальное количество дней, пока пользователь не сможет сменить пароль еще раз.</span><span class="sxs-lookup"><span data-stu-id="aa655-161">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="aa655-162">пассвордрекуирементсдескриптион</span><span class="sxs-lookup"><span data-stu-id="aa655-162">passwordRequirementsDescription</span></span>|<span data-ttu-id="aa655-163">String</span><span class="sxs-lookup"><span data-stu-id="aa655-163">String</span></span>|<span data-ttu-id="aa655-164">Получает или задает описание требований к сложности пароля.</span><span class="sxs-lookup"><span data-stu-id="aa655-164">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="aa655-165">рекуиреусерпресенце</span><span class="sxs-lookup"><span data-stu-id="aa655-165">requireUserPresence</span></span>|<span data-ttu-id="aa655-166">Логическое</span><span class="sxs-lookup"><span data-stu-id="aa655-166">Boolean</span></span>|<span data-ttu-id="aa655-167">Получает или задает значение, указывающее, требуется ли проверка подлинности с помощью идентификатора сенсорного экрана, идентификатора лица или секретного кода для доступа к записи цепочки ключей.</span><span class="sxs-lookup"><span data-stu-id="aa655-167">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="aa655-168">активедиректориситекоде</span><span class="sxs-lookup"><span data-stu-id="aa655-168">activeDirectorySiteCode</span></span>|<span data-ttu-id="aa655-169">String</span><span class="sxs-lookup"><span data-stu-id="aa655-169">String</span></span>|<span data-ttu-id="aa655-170">Получает или задает сайт Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa655-170">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="aa655-171">пассворденаблелокалсинк</span><span class="sxs-lookup"><span data-stu-id="aa655-171">passwordEnableLocalSync</span></span>|<span data-ttu-id="aa655-172">Логическое</span><span class="sxs-lookup"><span data-stu-id="aa655-172">Boolean</span></span>|<span data-ttu-id="aa655-173">Включает или отключает синхронизацию паролей.</span><span class="sxs-lookup"><span data-stu-id="aa655-173">Enables or disables password syncing.</span></span> <span data-ttu-id="aa655-174">Это не повлияет на пользователей, выполнивших вход в систему с помощью учетной записи мобильного устройства в macOS.</span><span class="sxs-lookup"><span data-stu-id="aa655-174">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="aa655-175">блоккактиведиректориситеаутодисковери</span><span class="sxs-lookup"><span data-stu-id="aa655-175">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="aa655-176">Логическое</span><span class="sxs-lookup"><span data-stu-id="aa655-176">Boolean</span></span>|<span data-ttu-id="aa655-177">Включает или отключает, может ли расширение Kerberos автоматически определять имя своего сайта.</span><span class="sxs-lookup"><span data-stu-id="aa655-177">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|
|<span data-ttu-id="aa655-178">пассвордчанжеурл</span><span class="sxs-lookup"><span data-stu-id="aa655-178">passwordChangeUrl</span></span>|<span data-ttu-id="aa655-179">String</span><span class="sxs-lookup"><span data-stu-id="aa655-179">String</span></span>|<span data-ttu-id="aa655-180">Получает или задает URL-адрес, на который будет отправляться пользователь при инициации смены пароля.</span><span class="sxs-lookup"><span data-stu-id="aa655-180">Gets or sets the URL that the user will be sent to when they initiate a password change.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa655-181">Связи</span><span class="sxs-lookup"><span data-stu-id="aa655-181">Relationships</span></span>
<span data-ttu-id="aa655-182">Нет</span><span class="sxs-lookup"><span data-stu-id="aa655-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa655-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa655-183">JSON Representation</span></span>
<span data-ttu-id="aa655-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa655-184">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
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




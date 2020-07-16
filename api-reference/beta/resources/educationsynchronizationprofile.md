---
title: Тип ресурса Едукатионсинчронизатионпрофиле
description: Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 05babeebb25130350e64d98ccfc408381547829e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790917"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="d138c-104">Тип ресурса Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="d138c-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="d138c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d138c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d138c-106">Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d138c-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="d138c-107">Этот ресурс предоставляет программное представление, используемое в [School Data Sync](https://sds.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="d138c-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="d138c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d138c-108">Methods</span></span>

| <span data-ttu-id="d138c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d138c-109">Method</span></span>                                                                    | <span data-ttu-id="d138c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d138c-110">Return Type</span></span>                                                 | <span data-ttu-id="d138c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d138c-111">Description</span></span>                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="d138c-112">Список профилей</span><span class="sxs-lookup"><span data-stu-id="d138c-112">List profiles</span></span>](../api/educationsynchronizationprofile-list.md)           | <span data-ttu-id="d138c-113">Коллекция [едукатионсинчронизатионпрофиле]</span><span class="sxs-lookup"><span data-stu-id="d138c-113">[educationSynchronizationProfile] collection</span></span>                | <span data-ttu-id="d138c-114">Получение списка всех профилей синхронизации в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d138c-114">Get a list of all the synchronization profiles in the tenant.</span></span>                                                                  |
| [<span data-ttu-id="d138c-115">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="d138c-115">Get profile</span></span>](../api/educationsynchronizationprofile-get.md)              | <span data-ttu-id="d138c-116">[едукатионсинчронизатионпрофиле]</span><span class="sxs-lookup"><span data-stu-id="d138c-116">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="d138c-117">Получение определенного профиля с учетом заданного идентификатора профиля.</span><span class="sxs-lookup"><span data-stu-id="d138c-117">Retrieve a specific profile given the profile identifier.</span></span>                                                                      |
| [<span data-ttu-id="d138c-118">Создание профиля</span><span class="sxs-lookup"><span data-stu-id="d138c-118">Create profile</span></span>](../api/educationsynchronizationprofile-post.md)          | <span data-ttu-id="d138c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d138c-119">None</span></span>                                                        | <span data-ttu-id="d138c-120">Создание нового профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-120">Create a new synchronization profile.</span></span>                                                                                          |
| [<span data-ttu-id="d138c-121">Удаление профиля</span><span class="sxs-lookup"><span data-stu-id="d138c-121">Delete profile</span></span>](../api/educationsynchronizationprofile-delete.md)        | <span data-ttu-id="d138c-122">[едукатионсинчронизатионпрофиле]</span><span class="sxs-lookup"><span data-stu-id="d138c-122">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="d138c-123">Удаление определенного профиля с учетом идентификатора профиля.</span><span class="sxs-lookup"><span data-stu-id="d138c-123">Delete a specific profile given the profile identifier.</span></span>                                                                        |
| [<span data-ttu-id="d138c-124">Приостановить профиль</span><span class="sxs-lookup"><span data-stu-id="d138c-124">Pause profile</span></span>](../api/educationsynchronizationprofile-pause.md)          | <span data-ttu-id="d138c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d138c-125">None</span></span>                                                        | <span data-ttu-id="d138c-126">Приостановите текущую синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="d138c-126">Pause an ongoing synchronization.</span></span>                                                                                              |
| [<span data-ttu-id="d138c-127">Профиль возобновления</span><span class="sxs-lookup"><span data-stu-id="d138c-127">Resume profile</span></span>](../api/educationsynchronizationprofile-resume.md)        | <span data-ttu-id="d138c-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d138c-128">None</span></span>                                                        | <span data-ttu-id="d138c-129">Возобновление приостановленной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-129">Resume a paused synchronization.</span></span>                                                                                               |
| [<span data-ttu-id="d138c-130">Сброс профиля</span><span class="sxs-lookup"><span data-stu-id="d138c-130">Reset profile</span></span>](../api/educationsynchronizationprofile-reset.md)          | <span data-ttu-id="d138c-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d138c-131">None</span></span>                                                        | <span data-ttu-id="d138c-132">Сбросьте состояние профиля и перезапустите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="d138c-132">Reset the state of the profile and restart synchronization.</span></span>                                                                    |
| [<span data-ttu-id="d138c-133">Начальный CSV-профиль</span><span class="sxs-lookup"><span data-stu-id="d138c-133">Start CSV profile</span></span>](../api/educationsynchronizationprofile-start.md)      | <span data-ttu-id="d138c-134">Коллекция [едукатионфилесинчронизатионверификатионмессаже]</span><span class="sxs-lookup"><span data-stu-id="d138c-134">[educationFileSynchronizationVerificationMessage]collection</span></span> | <span data-ttu-id="d138c-135">Проверьте отправленные исходные файлы и запустите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="d138c-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="d138c-136">Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер].</span><span class="sxs-lookup"><span data-stu-id="d138c-136">Applies only when the data provider is [educationCsvDataProvider].</span></span> |
| [<span data-ttu-id="d138c-137">Получение URL-адреса отправки CSV-файла</span><span class="sxs-lookup"><span data-stu-id="d138c-137">Get CSV upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="d138c-138">string</span><span class="sxs-lookup"><span data-stu-id="d138c-138">string</span></span>                                                      | <span data-ttu-id="d138c-139">Возвращает кратковременный URL-адрес для отправки CSV-файлов данных.</span><span class="sxs-lookup"><span data-stu-id="d138c-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="d138c-140">Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер].</span><span class="sxs-lookup"><span data-stu-id="d138c-140">Applies only when the data provider is [educationCsvDataProvider].</span></span>        |
| [<span data-ttu-id="d138c-141">Получение состояния</span><span class="sxs-lookup"><span data-stu-id="d138c-141">Get status</span></span>](../api/educationsynchronizationprofilestatus-get.md)         | <span data-ttu-id="d138c-142">[едукатионсинчронизатионпрофилестатус]</span><span class="sxs-lookup"><span data-stu-id="d138c-142">[educationsynchronizationProfileStatus]</span></span>                     | <span data-ttu-id="d138c-143">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-143">Return the status of a specific synchronization profile.</span></span>                                                                       |
| [<span data-ttu-id="d138c-144">Получение ошибок</span><span class="sxs-lookup"><span data-stu-id="d138c-144">Get errors</span></span>](../api/educationsynchronizationerrors-get.md)                | <span data-ttu-id="d138c-145">Коллекция [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="d138c-145">[educationSynchronizationError] collection</span></span>                  | <span data-ttu-id="d138c-146">Получение всех ошибок, возникших во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-146">Get all the errors generated during synchronization.</span></span>                                                                           |

## <a name="properties"></a><span data-ttu-id="d138c-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="d138c-147">Properties</span></span>

| <span data-ttu-id="d138c-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="d138c-148">Property</span></span>                             | <span data-ttu-id="d138c-149">Тип</span><span class="sxs-lookup"><span data-stu-id="d138c-149">Type</span></span>                                                   | <span data-ttu-id="d138c-150">Описание</span><span class="sxs-lookup"><span data-stu-id="d138c-150">Description</span></span>                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d138c-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d138c-151">displayName</span></span>                          | <span data-ttu-id="d138c-152">string</span><span class="sxs-lookup"><span data-stu-id="d138c-152">string</span></span>                                                 | <span data-ttu-id="d138c-153">Имя профиля конфигурации для удостоверений синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-153">Name of the configuration profile for syncing identities.</span></span>                                                                         |
| <span data-ttu-id="d138c-154">Предоставление dataProvider</span><span class="sxs-lookup"><span data-stu-id="d138c-154">dataProvider</span></span>                         | <span data-ttu-id="d138c-155">[едукатионсинчронизатиондатапровидер]</span><span class="sxs-lookup"><span data-stu-id="d138c-155">[educationSynchronizationDataProvider]</span></span>                 | <span data-ttu-id="d138c-156">Поставщик данных, используемый для профиля.</span><span class="sxs-lookup"><span data-stu-id="d138c-156">The data provider used for the profile.</span></span>                                                                                           |
| <span data-ttu-id="d138c-157">идентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d138c-157">identitySynchronizationConfiguration</span></span> | <span data-ttu-id="d138c-158">[едукатионидентитисинчронизатионконфигуратион]</span><span class="sxs-lookup"><span data-stu-id="d138c-158">[educationIdentitySynchronizationConfiguration]</span></span>        | <span data-ttu-id="d138c-159">Определяет, как профиль должен [создавать новые][fullsync] или [сопоставляться с имеющимися][dirsync] пользователями AAD.</span><span class="sxs-lookup"><span data-stu-id="d138c-159">Determines how the Profile should [create new][fullsync] or [match existing][dirsync] AAD Users.</span></span>                                  |
| <span data-ttu-id="d138c-160">лиценсестоассигн</span><span class="sxs-lookup"><span data-stu-id="d138c-160">licensesToAssign</span></span>                     | <span data-ttu-id="d138c-161">Коллекция [едукатионсинчронизатионлиценсеассигнмент]</span><span class="sxs-lookup"><span data-stu-id="d138c-161">[educationSynchronizationLicenseAssignment] collection</span></span> | <span data-ttu-id="d138c-162">Конфигурация установки лицензий.</span><span class="sxs-lookup"><span data-stu-id="d138c-162">License setup configuration.</span></span>                                                                                                      |
| <span data-ttu-id="d138c-163">state</span><span class="sxs-lookup"><span data-stu-id="d138c-163">state</span></span>                                | <span data-ttu-id="d138c-164">едукатионсинчронизатионпрофилестате</span><span class="sxs-lookup"><span data-stu-id="d138c-164">educationSynchronizationProfileState</span></span>                   | <span data-ttu-id="d138c-165">Состояние профиля.</span><span class="sxs-lookup"><span data-stu-id="d138c-165">The state of the profile.</span></span> <span data-ttu-id="d138c-166">Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span><span class="sxs-lookup"><span data-stu-id="d138c-166">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d138c-167">Связи</span><span class="sxs-lookup"><span data-stu-id="d138c-167">Relationships</span></span>

| <span data-ttu-id="d138c-168">Связь</span><span class="sxs-lookup"><span data-stu-id="d138c-168">Relationship</span></span>  | <span data-ttu-id="d138c-169">Тип</span><span class="sxs-lookup"><span data-stu-id="d138c-169">Type</span></span>                                       | <span data-ttu-id="d138c-170">Описание</span><span class="sxs-lookup"><span data-stu-id="d138c-170">Description</span></span>                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| <span data-ttu-id="d138c-171">ошибки</span><span class="sxs-lookup"><span data-stu-id="d138c-171">errors</span></span>        | <span data-ttu-id="d138c-172">Коллекция [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="d138c-172">[educationSynchronizationError] collection</span></span> | <span data-ttu-id="d138c-173">Все ошибки, связанные с этим профилем синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-173">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="d138c-174">профилестатус</span><span class="sxs-lookup"><span data-stu-id="d138c-174">profileStatus</span></span> | <span data-ttu-id="d138c-175">[едукатионсинчронизатионпрофилестатус]</span><span class="sxs-lookup"><span data-stu-id="d138c-175">[educationSynchronizationProfileStatus]</span></span>    | <span data-ttu-id="d138c-176">Состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-176">The synchronization status.</span></span>                              |

## <a name="data-providers"></a><span data-ttu-id="d138c-177">Data Providers</span><span class="sxs-lookup"><span data-stu-id="d138c-177">Data Providers</span></span>

<span data-ttu-id="d138c-178">Каждый [едукатионсинчронизатионпрофиле] должен указать одного из указанных ниже поставщиков данных, который будет использоваться в качестве источника синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d138c-178">Each [educationSynchronizationProfile] must specify one of the follow data providers to use as the synchronization source.</span></span>

| <span data-ttu-id="d138c-179">Поставщик данных</span><span class="sxs-lookup"><span data-stu-id="d138c-179">Data Provider</span></span>                       | <span data-ttu-id="d138c-180">Описание</span><span class="sxs-lookup"><span data-stu-id="d138c-180">Description</span></span>                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d138c-181">[едукатионксвдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="d138c-181">[educationCsvDataProvider]</span></span>          | <span data-ttu-id="d138c-182">CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md)</span><span class="sxs-lookup"><span data-stu-id="d138c-182">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="d138c-183">едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="d138c-183">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="d138c-184">API OneRoster 1.1</span><span class="sxs-lookup"><span data-stu-id="d138c-184">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="d138c-185">[едукатионповерсчулдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="d138c-185">[educationPowerSchoolDataProvider]</span></span>  | <span data-ttu-id="d138c-186">API PowerSchool</span><span class="sxs-lookup"><span data-stu-id="d138c-186">PowerSchool API</span></span>                                                                                    |

## <a name="json-representation"></a><span data-ttu-id="d138c-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d138c-187">JSON representation</span></span>

<span data-ttu-id="d138c-188">Ниже представлено представление ресурса **едукатионсинчронизатионпрофиле** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d138c-188">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "state": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileState"
  },
  "profileStatus": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
  },
  "errors": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
    }
  ],
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationCsvDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "handleSpecialCharacterConstraint": "Boolean"
}
```

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[educationsynchronizationprofile]: educationsynchronizationprofile.md
[едукатионсинчронизатионпрофилестатус]: educationsynchronizationProfileStatus.md
[educationsynchronizationprofilestatus]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[едукатионфилесинчронизатионверификатионмессаже]: educationFileSynchronizationVerificationMessage.md
[educationfilesynchronizationverificationmessage]: educationFileSynchronizationVerificationMessage.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[едукатионсинчронизатиондатапровидер]: educationSynchronizationDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[едукатионидентитисинчронизатионконфигуратион]: educationIdentitySynchronizationConfiguration.md
[educationidentitysynchronizationconfiguration]: educationIdentitySynchronizationConfiguration.md
[едукатионсинчронизатионлиценсеассигнмент]: educationSynchronizationLicenseAssignment.md
[educationsynchronizationlicenseassignment]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationSynchronizationProfile/dataProvider:\r\n      Referenced type microsoft.graph.educationSynchronizationDataProvider is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->

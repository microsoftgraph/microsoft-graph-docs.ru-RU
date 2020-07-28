---
title: Тип ресурса Едукатионсинчронизатионпрофиле
description: Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 86c8189e170bba5899f82f75902dfe68dd0d3fd1
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434916"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="bca99-104">Тип ресурса Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="bca99-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="bca99-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bca99-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bca99-106">Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bca99-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="bca99-107">Этот ресурс предоставляет программное представление, используемое в [School Data Sync](https://sds.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="bca99-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="bca99-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bca99-108">Methods</span></span>

| <span data-ttu-id="bca99-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bca99-109">Method</span></span>                                                                    | <span data-ttu-id="bca99-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bca99-110">Return Type</span></span>                                                 | <span data-ttu-id="bca99-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bca99-111">Description</span></span>                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="bca99-112">Список профилей</span><span class="sxs-lookup"><span data-stu-id="bca99-112">List profiles</span></span>](../api/educationsynchronizationprofile-list.md)           | <span data-ttu-id="bca99-113">Коллекция [едукатионсинчронизатионпрофиле]</span><span class="sxs-lookup"><span data-stu-id="bca99-113">[educationSynchronizationProfile] collection</span></span>                | <span data-ttu-id="bca99-114">Получение списка всех профилей синхронизации в клиенте.</span><span class="sxs-lookup"><span data-stu-id="bca99-114">Get a list of all the synchronization profiles in the tenant.</span></span>                                                                  |
| [<span data-ttu-id="bca99-115">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="bca99-115">Get profile</span></span>](../api/educationsynchronizationprofile-get.md)              | <span data-ttu-id="bca99-116">[едукатионсинчронизатионпрофиле]</span><span class="sxs-lookup"><span data-stu-id="bca99-116">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="bca99-117">Получение определенного профиля с учетом заданного идентификатора профиля.</span><span class="sxs-lookup"><span data-stu-id="bca99-117">Retrieve a specific profile given the profile identifier.</span></span>                                                                      |
| [<span data-ttu-id="bca99-118">Создание профиля</span><span class="sxs-lookup"><span data-stu-id="bca99-118">Create profile</span></span>](../api/educationsynchronizationprofile-post.md)          | <span data-ttu-id="bca99-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bca99-119">None</span></span>                                                        | <span data-ttu-id="bca99-120">Создание нового профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-120">Create a new synchronization profile.</span></span>                                                                                          |
| [<span data-ttu-id="bca99-121">Удаление профиля</span><span class="sxs-lookup"><span data-stu-id="bca99-121">Delete profile</span></span>](../api/educationsynchronizationprofile-delete.md)        | <span data-ttu-id="bca99-122">[едукатионсинчронизатионпрофиле]</span><span class="sxs-lookup"><span data-stu-id="bca99-122">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="bca99-123">Удаление определенного профиля с учетом идентификатора профиля.</span><span class="sxs-lookup"><span data-stu-id="bca99-123">Delete a specific profile given the profile identifier.</span></span>                                                                        |
| [<span data-ttu-id="bca99-124">Приостановить профиль</span><span class="sxs-lookup"><span data-stu-id="bca99-124">Pause profile</span></span>](../api/educationsynchronizationprofile-pause.md)          | <span data-ttu-id="bca99-125">Нет</span><span class="sxs-lookup"><span data-stu-id="bca99-125">None</span></span>                                                        | <span data-ttu-id="bca99-126">Приостановите текущую синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="bca99-126">Pause an ongoing synchronization.</span></span>                                                                                              |
| [<span data-ttu-id="bca99-127">Профиль возобновления</span><span class="sxs-lookup"><span data-stu-id="bca99-127">Resume profile</span></span>](../api/educationsynchronizationprofile-resume.md)        | <span data-ttu-id="bca99-128">Нет</span><span class="sxs-lookup"><span data-stu-id="bca99-128">None</span></span>                                                        | <span data-ttu-id="bca99-129">Возобновление приостановленной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-129">Resume a paused synchronization.</span></span>                                                                                               |
| [<span data-ttu-id="bca99-130">Сброс профиля</span><span class="sxs-lookup"><span data-stu-id="bca99-130">Reset profile</span></span>](../api/educationsynchronizationprofile-reset.md)          | <span data-ttu-id="bca99-131">Нет</span><span class="sxs-lookup"><span data-stu-id="bca99-131">None</span></span>                                                        | <span data-ttu-id="bca99-132">Сбросьте состояние профиля и перезапустите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="bca99-132">Reset the state of the profile and restart synchronization.</span></span>                                                                    |
| [<span data-ttu-id="bca99-133">Начальный CSV-профиль</span><span class="sxs-lookup"><span data-stu-id="bca99-133">Start CSV profile</span></span>](../api/educationsynchronizationprofile-start.md)      | <span data-ttu-id="bca99-134">Коллекция [едукатионфилесинчронизатионверификатионмессаже]</span><span class="sxs-lookup"><span data-stu-id="bca99-134">[educationFileSynchronizationVerificationMessage]collection</span></span> | <span data-ttu-id="bca99-135">Проверьте отправленные исходные файлы и запустите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="bca99-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="bca99-136">Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер].</span><span class="sxs-lookup"><span data-stu-id="bca99-136">Applies only when the data provider is [educationCsvDataProvider].</span></span> |
| [<span data-ttu-id="bca99-137">Получение URL-адреса отправки CSV-файла</span><span class="sxs-lookup"><span data-stu-id="bca99-137">Get CSV upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="bca99-138">Строка</span><span class="sxs-lookup"><span data-stu-id="bca99-138">string</span></span>                                                      | <span data-ttu-id="bca99-139">Возвращает кратковременный URL-адрес для отправки CSV-файлов данных.</span><span class="sxs-lookup"><span data-stu-id="bca99-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="bca99-140">Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер].</span><span class="sxs-lookup"><span data-stu-id="bca99-140">Applies only when the data provider is [educationCsvDataProvider].</span></span>        |
| [<span data-ttu-id="bca99-141">Получение состояния</span><span class="sxs-lookup"><span data-stu-id="bca99-141">Get status</span></span>](../api/educationsynchronizationprofilestatus-get.md)         | <span data-ttu-id="bca99-142">[едукатионсинчронизатионпрофилестатус]</span><span class="sxs-lookup"><span data-stu-id="bca99-142">[educationsynchronizationProfileStatus]</span></span>                     | <span data-ttu-id="bca99-143">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-143">Return the status of a specific synchronization profile.</span></span>                                                                       |
| [<span data-ttu-id="bca99-144">Получение ошибок</span><span class="sxs-lookup"><span data-stu-id="bca99-144">Get errors</span></span>](../api/educationsynchronizationerrors-get.md)                | <span data-ttu-id="bca99-145">Коллекция [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="bca99-145">[educationSynchronizationError] collection</span></span>                  | <span data-ttu-id="bca99-146">Получение всех ошибок, возникших во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-146">Get all the errors generated during synchronization.</span></span>                                                                           |

## <a name="properties"></a><span data-ttu-id="bca99-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="bca99-147">Properties</span></span>

| <span data-ttu-id="bca99-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="bca99-148">Property</span></span>                             | <span data-ttu-id="bca99-149">Тип</span><span class="sxs-lookup"><span data-stu-id="bca99-149">Type</span></span>                                                   | <span data-ttu-id="bca99-150">Описание</span><span class="sxs-lookup"><span data-stu-id="bca99-150">Description</span></span>                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bca99-151">id</span><span class="sxs-lookup"><span data-stu-id="bca99-151">id</span></span>                                   | <span data-ttu-id="bca99-152">String</span><span class="sxs-lookup"><span data-stu-id="bca99-152">String</span></span>                                                 | <span data-ttu-id="bca99-153">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="bca99-153">The unique identifier for the resource.</span></span> <span data-ttu-id="bca99-154">(только для чтения)</span><span class="sxs-lookup"><span data-stu-id="bca99-154">(read-only)</span></span>                                                                               |
| <span data-ttu-id="bca99-155">displayName</span><span class="sxs-lookup"><span data-stu-id="bca99-155">displayName</span></span>                          | <span data-ttu-id="bca99-156">Строка</span><span class="sxs-lookup"><span data-stu-id="bca99-156">String</span></span>                                                 | <span data-ttu-id="bca99-157">Имя профиля конфигурации для удостоверений синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-157">Name of the configuration profile for syncing identities.</span></span>                                                                         |
| <span data-ttu-id="bca99-158">Предоставление dataProvider</span><span class="sxs-lookup"><span data-stu-id="bca99-158">dataProvider</span></span>                         | <span data-ttu-id="bca99-159">[едукатионсинчронизатиондатапровидер]</span><span class="sxs-lookup"><span data-stu-id="bca99-159">[educationSynchronizationDataProvider]</span></span>                 | <span data-ttu-id="bca99-160">Поставщик данных, используемый для профиля.</span><span class="sxs-lookup"><span data-stu-id="bca99-160">The data provider used for the profile.</span></span>                                                                                           |
| <span data-ttu-id="bca99-161">expirationDate</span><span class="sxs-lookup"><span data-stu-id="bca99-161">expirationDate</span></span>                       | <span data-ttu-id="bca99-162">Дата</span><span class="sxs-lookup"><span data-stu-id="bca99-162">Date</span></span>                                                   | <span data-ttu-id="bca99-163">Дата истечения срока действия профиля и прекращение синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-163">The date the profile should be considered expired and cease syncing.</span></span> <span data-ttu-id="bca99-164">Когда `null` .</span><span class="sxs-lookup"><span data-stu-id="bca99-164">When `null`.</span></span> <span data-ttu-id="bca99-165">срок действия профиля никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="bca99-165">the profile will never expire.</span></span> <span data-ttu-id="bca99-166">(необязательный)</span><span class="sxs-lookup"><span data-stu-id="bca99-166">(optional)</span></span>       |
| <span data-ttu-id="bca99-167">хандлеспеЦиалчарактерконстраинт</span><span class="sxs-lookup"><span data-stu-id="bca99-167">handleSpecialCharacterConstraint</span></span>     | <span data-ttu-id="bca99-168">Логический</span><span class="sxs-lookup"><span data-stu-id="bca99-168">Bool</span></span>                                                   | <span data-ttu-id="bca99-169">Определяет, должно ли учебная синхронизация данных автоматически заменять неподдерживаемые специальные символы при синхронизации из источника.</span><span class="sxs-lookup"><span data-stu-id="bca99-169">Determines if School Data Sync should automatically replace unsupported special characters while syncing from source.</span></span>             |
| <span data-ttu-id="bca99-170">идентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bca99-170">identitySynchronizationConfiguration</span></span> | <span data-ttu-id="bca99-171">[едукатионидентитисинчронизатионконфигуратион]</span><span class="sxs-lookup"><span data-stu-id="bca99-171">[educationIdentitySynchronizationConfiguration]</span></span>        | <span data-ttu-id="bca99-172">Определяет, как профиль должен [создавать новые][fullsync] или [сопоставляться с имеющимися][dirsync] пользователями AAD.</span><span class="sxs-lookup"><span data-stu-id="bca99-172">Determines how the Profile should [create new][fullsync] or [match existing][dirsync] AAD Users.</span></span>                                  |
| <span data-ttu-id="bca99-173">лиценсестоассигн</span><span class="sxs-lookup"><span data-stu-id="bca99-173">licensesToAssign</span></span>                     | <span data-ttu-id="bca99-174">Коллекция [едукатионсинчронизатионлиценсеассигнмент]</span><span class="sxs-lookup"><span data-stu-id="bca99-174">[educationSynchronizationLicenseAssignment] collection</span></span> | <span data-ttu-id="bca99-175">Конфигурация установки лицензий.</span><span class="sxs-lookup"><span data-stu-id="bca99-175">License setup configuration.</span></span>                                                                                                      |
| <span data-ttu-id="bca99-176">state</span><span class="sxs-lookup"><span data-stu-id="bca99-176">state</span></span>                                | <span data-ttu-id="bca99-177">едукатионсинчронизатионпрофилестате</span><span class="sxs-lookup"><span data-stu-id="bca99-177">educationSynchronizationProfileState</span></span>                   | <span data-ttu-id="bca99-178">Состояние профиля.</span><span class="sxs-lookup"><span data-stu-id="bca99-178">The state of the profile.</span></span> <span data-ttu-id="bca99-179">Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span><span class="sxs-lookup"><span data-stu-id="bca99-179">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bca99-180">Связи</span><span class="sxs-lookup"><span data-stu-id="bca99-180">Relationships</span></span>

| <span data-ttu-id="bca99-181">Связь</span><span class="sxs-lookup"><span data-stu-id="bca99-181">Relationship</span></span>  | <span data-ttu-id="bca99-182">Тип</span><span class="sxs-lookup"><span data-stu-id="bca99-182">Type</span></span>                                       | <span data-ttu-id="bca99-183">Описание</span><span class="sxs-lookup"><span data-stu-id="bca99-183">Description</span></span>                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| <span data-ttu-id="bca99-184">ошибки</span><span class="sxs-lookup"><span data-stu-id="bca99-184">errors</span></span>        | <span data-ttu-id="bca99-185">Коллекция [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="bca99-185">[educationSynchronizationError] collection</span></span> | <span data-ttu-id="bca99-186">Все ошибки, связанные с этим профилем синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-186">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="bca99-187">профилестатус</span><span class="sxs-lookup"><span data-stu-id="bca99-187">profileStatus</span></span> | <span data-ttu-id="bca99-188">[едукатионсинчронизатионпрофилестатус]</span><span class="sxs-lookup"><span data-stu-id="bca99-188">[educationSynchronizationProfileStatus]</span></span>    | <span data-ttu-id="bca99-189">Состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-189">The synchronization status.</span></span>                              |

## <a name="data-providers"></a><span data-ttu-id="bca99-190">Data Providers</span><span class="sxs-lookup"><span data-stu-id="bca99-190">Data Providers</span></span>

<span data-ttu-id="bca99-191">Каждый [едукатионсинчронизатионпрофиле] должен указать одного из указанных ниже поставщиков данных, который будет использоваться в качестве источника синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bca99-191">Each [educationSynchronizationProfile] must specify one of the follow data providers to use as the synchronization source.</span></span>

| <span data-ttu-id="bca99-192">Поставщик данных</span><span class="sxs-lookup"><span data-stu-id="bca99-192">Data Provider</span></span>                                                             | <span data-ttu-id="bca99-193">Описание</span><span class="sxs-lookup"><span data-stu-id="bca99-193">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bca99-194">[едукатионксвдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="bca99-194">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="bca99-195">CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md)</span><span class="sxs-lookup"><span data-stu-id="bca99-195">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="bca99-196">едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="bca99-196">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="bca99-197">API OneRoster 1.1</span><span class="sxs-lookup"><span data-stu-id="bca99-197">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="bca99-198">[едукатионповерсчулдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="bca99-198">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="bca99-199">API PowerSchool</span><span class="sxs-lookup"><span data-stu-id="bca99-199">PowerSchool API</span></span>                                                                                    |

## <a name="json-representation"></a><span data-ttu-id="bca99-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bca99-200">JSON representation</span></span>

<span data-ttu-id="bca99-201">Ниже представлено представление ресурса **едукатионсинчронизатионпрофиле** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bca99-201">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

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
  "handleSpecialCharacterConstraint": "Boolean",
  "expirationDate": "Date"
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

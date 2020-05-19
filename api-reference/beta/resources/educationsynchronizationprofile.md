---
title: Тип ресурса Едукатионсинчронизатионпрофиле
description: Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c498abb711a336f3627ef0b63e6c742e633ea05a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289937"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="96b3b-104">Тип ресурса Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="96b3b-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="96b3b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96b3b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96b3b-106">Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="96b3b-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="96b3b-107">Этот ресурс предоставляет программное представление, используемое в [School Data Sync](https://sds.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="96b3b-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="96b3b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="96b3b-108">Methods</span></span>

| <span data-ttu-id="96b3b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="96b3b-109">Method</span></span> | <span data-ttu-id="96b3b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="96b3b-110">Return Type</span></span> | <span data-ttu-id="96b3b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="96b3b-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="96b3b-112">Профили синхронизации списка</span><span class="sxs-lookup"><span data-stu-id="96b3b-112">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md) | <span data-ttu-id="96b3b-113">Коллекция **едукатионсинчронизатионпрофиле**</span><span class="sxs-lookup"><span data-stu-id="96b3b-113">**educationSynchronizationProfile** collection</span></span> | <span data-ttu-id="96b3b-114">Получение списка всех профилей синхронизации в клиенте.</span><span class="sxs-lookup"><span data-stu-id="96b3b-114">Get a list of all the synchronization profiles in the tenant.</span></span> |
| [<span data-ttu-id="96b3b-115">Получение профиля синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-115">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md) | <span data-ttu-id="96b3b-116">**едукатионсинчронизатионпрофиле**</span><span class="sxs-lookup"><span data-stu-id="96b3b-116">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="96b3b-117">Получение определенного профиля с учетом заданного идентификатора профиля.</span><span class="sxs-lookup"><span data-stu-id="96b3b-117">Retrieve a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="96b3b-118">Создание профиля синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-118">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md) | <span data-ttu-id="96b3b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="96b3b-119">None</span></span> | <span data-ttu-id="96b3b-120">Создание нового профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96b3b-120">Create a new synchronization profile.</span></span> |
| [<span data-ttu-id="96b3b-121">Удаление профиля синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-121">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md) | <span data-ttu-id="96b3b-122">**едукатионсинчронизатионпрофиле**</span><span class="sxs-lookup"><span data-stu-id="96b3b-122">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="96b3b-123">Удаление определенного профиля с учетом идентификатора профиля.</span><span class="sxs-lookup"><span data-stu-id="96b3b-123">Delete a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="96b3b-124">Приостановка текущей синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-124">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md) | <span data-ttu-id="96b3b-125">Нет</span><span class="sxs-lookup"><span data-stu-id="96b3b-125">None</span></span> | <span data-ttu-id="96b3b-126">Приостановите текущую синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="96b3b-126">Pause an ongoing synchronization.</span></span> |
| [<span data-ttu-id="96b3b-127">Возобновление приостановленной синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-127">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md) | <span data-ttu-id="96b3b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="96b3b-128">None</span></span> | <span data-ttu-id="96b3b-129">Возобновление приостановленной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96b3b-129">Resume a paused synchronization.</span></span> |
| [<span data-ttu-id="96b3b-130">Сброс синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-130">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md) | <span data-ttu-id="96b3b-131">Нет</span><span class="sxs-lookup"><span data-stu-id="96b3b-131">None</span></span> | <span data-ttu-id="96b3b-132">Сбросьте состояние профиля и перезапустите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="96b3b-132">Reset the state of the profile and restart synchronization.</span></span> |
| [<span data-ttu-id="96b3b-133">Запуск синхронизации для отправленных файлов</span><span class="sxs-lookup"><span data-stu-id="96b3b-133">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) | <span data-ttu-id="96b3b-134">Коллекция [едукатионфилесинчронизатионверификатионмессаже](educationfilesynchronizationverificationmessage.md)</span><span class="sxs-lookup"><span data-stu-id="96b3b-134">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) collection</span></span>| <span data-ttu-id="96b3b-135">Проверьте отправленные исходные файлы и запустите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="96b3b-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="96b3b-136">Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер](educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="96b3b-136">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="96b3b-137">Получение URL-адреса отправки</span><span class="sxs-lookup"><span data-stu-id="96b3b-137">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="96b3b-138">string</span><span class="sxs-lookup"><span data-stu-id="96b3b-138">string</span></span> | <span data-ttu-id="96b3b-139">Возвращает кратковременный URL-адрес для отправки CSV-файлов данных.</span><span class="sxs-lookup"><span data-stu-id="96b3b-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="96b3b-140">Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер](educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="96b3b-140">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="96b3b-141">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-141">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | [<span data-ttu-id="96b3b-142">status</span><span class="sxs-lookup"><span data-stu-id="96b3b-142">status</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="96b3b-143">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96b3b-143">Return the status of a specific synchronization profile.</span></span> |
| [<span data-ttu-id="96b3b-144">Получение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="96b3b-144">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="96b3b-145">Коллекция [educationSynchronizationError](educationsynchronizationerror.md)</span><span class="sxs-lookup"><span data-stu-id="96b3b-145">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="96b3b-146">Получение всех ошибок, возникших во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96b3b-146">Get all the errors generated during synchronization.</span></span> |

## <a name="properties"></a><span data-ttu-id="96b3b-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="96b3b-147">Properties</span></span>

| <span data-ttu-id="96b3b-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="96b3b-148">Property</span></span> | <span data-ttu-id="96b3b-149">Тип</span><span class="sxs-lookup"><span data-stu-id="96b3b-149">Type</span></span> | <span data-ttu-id="96b3b-150">Описание</span><span class="sxs-lookup"><span data-stu-id="96b3b-150">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="96b3b-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="96b3b-151">**displayName**</span></span> | <span data-ttu-id="96b3b-152">string</span><span class="sxs-lookup"><span data-stu-id="96b3b-152">string</span></span> |  <span data-ttu-id="96b3b-153">Имя профиля конфигурации для удостоверений синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96b3b-153">Name of the configuration profile for syncing identities.</span></span>         |
| <span data-ttu-id="96b3b-154">**Предоставление dataProvider**</span><span class="sxs-lookup"><span data-stu-id="96b3b-154">**dataProvider**</span></span> | [<span data-ttu-id="96b3b-155">едукатионсинчронизатиондатапровидер</span><span class="sxs-lookup"><span data-stu-id="96b3b-155">educationSynchronizationDataProvider</span></span>](educationsynchronizationdataprovider.md) |  <span data-ttu-id="96b3b-156">Поставщик данных, используемый для профиля.</span><span class="sxs-lookup"><span data-stu-id="96b3b-156">The data provider used for the profile.</span></span>         |
| <span data-ttu-id="96b3b-157">**идентитисинчронизатионконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="96b3b-157">**identitySynchronizationConfiguration**</span></span> | [<span data-ttu-id="96b3b-158">едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="96b3b-158">educationIdentitySynchronizationConfiguration</span></span>](educationidentitysynchronizationconfiguration.md) | <span data-ttu-id="96b3b-159">[Создание](educationidentitycreationconfiguration.md) удостоверения или [соответствующая](educationidentitymatchingconfiguration.md) конфигурация.</span><span class="sxs-lookup"><span data-stu-id="96b3b-159">Identity [creation](educationidentitycreationconfiguration.md) or [matching](educationidentitymatchingconfiguration.md) configuration .</span></span>        |
| <span data-ttu-id="96b3b-160">**лиценсестоассигн**</span><span class="sxs-lookup"><span data-stu-id="96b3b-160">**licensesToAssign**</span></span> | <span data-ttu-id="96b3b-161">Коллекция [едукатионсинчронизатионлиценсеассигнмент](educationsynchronizationlicenseassignment.md)</span><span class="sxs-lookup"><span data-stu-id="96b3b-161">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) collection</span></span>|  <span data-ttu-id="96b3b-162">Конфигурация установки лицензий.</span><span class="sxs-lookup"><span data-stu-id="96b3b-162">License setup configuration.</span></span>        |
| <span data-ttu-id="96b3b-163">**state**</span><span class="sxs-lookup"><span data-stu-id="96b3b-163">**state**</span></span> | <span data-ttu-id="96b3b-164">едукатионсинчронизатионпрофилестате</span><span class="sxs-lookup"><span data-stu-id="96b3b-164">educationSynchronizationProfileState</span></span> |  <span data-ttu-id="96b3b-165">Состояние профиля.</span><span class="sxs-lookup"><span data-stu-id="96b3b-165">The state of the profile.</span></span> <span data-ttu-id="96b3b-166">Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span><span class="sxs-lookup"><span data-stu-id="96b3b-166">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span>          |

## <a name="relationships"></a><span data-ttu-id="96b3b-167">Отношения</span><span class="sxs-lookup"><span data-stu-id="96b3b-167">Relationships</span></span>

| <span data-ttu-id="96b3b-168">Свойство</span><span class="sxs-lookup"><span data-stu-id="96b3b-168">Property</span></span> | <span data-ttu-id="96b3b-169">Тип</span><span class="sxs-lookup"><span data-stu-id="96b3b-169">Type</span></span> | <span data-ttu-id="96b3b-170">Описание</span><span class="sxs-lookup"><span data-stu-id="96b3b-170">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="96b3b-171">**errors**</span><span class="sxs-lookup"><span data-stu-id="96b3b-171">**errors**</span></span> | <span data-ttu-id="96b3b-172">Коллекция [educationSynchronizationError](educationsynchronizationerror.md)</span><span class="sxs-lookup"><span data-stu-id="96b3b-172">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="96b3b-173">Все ошибки, связанные с этим профилем синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96b3b-173">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="96b3b-174">**профилестатус**</span><span class="sxs-lookup"><span data-stu-id="96b3b-174">**profileStatus**</span></span> | [<span data-ttu-id="96b3b-175">едукатионсинчронизатионпрофилестатус</span><span class="sxs-lookup"><span data-stu-id="96b3b-175">educationSynchronizationProfileStatus</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="96b3b-176">Состояние синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96b3b-176">The synchronization status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96b3b-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96b3b-177">JSON representation</span></span>
<span data-ttu-id="96b3b-178">Ниже представлено представление ресурса **едукатионсинчронизатионпрофиле** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96b3b-178">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

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
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```

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
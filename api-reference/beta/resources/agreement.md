---
title: тип ресурса соглашения
description: Представляет настраиваемые условия соглашения об использовании клиента, созданного и управляемого с помощью Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: bb1de9d03de4d891ef91d076ccbd41e6b569e3f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433203"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="8ccd1-103">тип ресурса соглашения</span><span class="sxs-lookup"><span data-stu-id="8ccd1-103">agreement resource type</span></span>

<span data-ttu-id="8ccd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ccd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ccd1-105">Представляет настраиваемые условия соглашения об использовании клиента, созданного и управляемого с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8ccd1-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="8ccd1-106">Вы можете использовать следующие методы для создания и управления функцией [Azure Active Directory Terms of Use](/azure/active-directory/active-directory-tou) в соответствии с вашим сценарием.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="8ccd1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8ccd1-107">Methods</span></span>

| <span data-ttu-id="8ccd1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8ccd1-108">Method</span></span>       | <span data-ttu-id="8ccd1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ccd1-109">Return Type</span></span> | <span data-ttu-id="8ccd1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8ccd1-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8ccd1-111">Создание соглашений</span><span class="sxs-lookup"><span data-stu-id="8ccd1-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="8ccd1-112">соглашение</span><span class="sxs-lookup"><span data-stu-id="8ccd1-112">agreement</span></span>](agreement.md) | <span data-ttu-id="8ccd1-113">Создайте новое соглашение, разместив в коллекции соглашений.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="8ccd1-114">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="8ccd1-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="8ccd1-115">[коллекция соглашений](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="8ccd1-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="8ccd1-116">Получите коллекцию объектов соглашения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="8ccd1-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="8ccd1-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="8ccd1-118">соглашение</span><span class="sxs-lookup"><span data-stu-id="8ccd1-118">agreement</span></span>](agreement.md) | <span data-ttu-id="8ccd1-119">Чтение свойств и связей объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="8ccd1-120">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="8ccd1-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="8ccd1-121">соглашение</span><span class="sxs-lookup"><span data-stu-id="8ccd1-121">agreement</span></span>](agreement.md) | <span data-ttu-id="8ccd1-122">Обновление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="8ccd1-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="8ccd1-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="8ccd1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8ccd1-124">None</span></span> | <span data-ttu-id="8ccd1-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="8ccd1-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ccd1-126">Properties</span></span>
| <span data-ttu-id="8ccd1-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ccd1-127">Property</span></span>     | <span data-ttu-id="8ccd1-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8ccd1-128">Type</span></span>        | <span data-ttu-id="8ccd1-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8ccd1-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ccd1-130">displayName</span><span class="sxs-lookup"><span data-stu-id="8ccd1-130">displayName</span></span>|<span data-ttu-id="8ccd1-131">String</span><span class="sxs-lookup"><span data-stu-id="8ccd1-131">String</span></span>|<span data-ttu-id="8ccd1-132">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-132">Display name of the agreement.</span></span> <span data-ttu-id="8ccd1-133">Имя отображения используется для внутреннего отслеживания соглашения, но не отображается конечным пользователям, которые просматривают соглашение.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="8ccd1-134">id</span><span class="sxs-lookup"><span data-stu-id="8ccd1-134">id</span></span>|<span data-ttu-id="8ccd1-135">String</span><span class="sxs-lookup"><span data-stu-id="8ccd1-135">String</span></span>| <span data-ttu-id="8ccd1-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-136">Read-only.</span></span>|
|<span data-ttu-id="8ccd1-137">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="8ccd1-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="8ccd1-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ccd1-138">Boolean</span></span>|<span data-ttu-id="8ccd1-139">Этот параметр позволяет требовать от конечных пользователей принять это соглашение на каждом устройстве, с которое они имеют к нему доступ.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="8ccd1-140">Конечный пользователь должен будет зарегистрировать свое устройство в Azure AD, если он этого еще не сделал.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="8ccd1-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="8ccd1-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="8ccd1-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ccd1-142">Boolean</span></span>|<span data-ttu-id="8ccd1-143">Указывает, должен ли пользователь расширить соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="8ccd1-144">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="8ccd1-144">termsExpiration</span></span>|[<span data-ttu-id="8ccd1-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="8ccd1-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="8ccd1-146">Срок действия и периодичность соглашения для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="8ccd1-147">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="8ccd1-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="8ccd1-148">Duration</span><span class="sxs-lookup"><span data-stu-id="8ccd1-148">Duration</span></span>|<span data-ttu-id="8ccd1-149">Продолжительность, после которой пользователь должен повторно принять условия использования.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="8ccd1-150">Значение представлено в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8ccd1-151">Связи</span><span class="sxs-lookup"><span data-stu-id="8ccd1-151">Relationships</span></span>
| <span data-ttu-id="8ccd1-152">Связь</span><span class="sxs-lookup"><span data-stu-id="8ccd1-152">Relationship</span></span> | <span data-ttu-id="8ccd1-153">Тип</span><span class="sxs-lookup"><span data-stu-id="8ccd1-153">Type</span></span>        | <span data-ttu-id="8ccd1-154">Описание</span><span class="sxs-lookup"><span data-stu-id="8ccd1-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ccd1-155">приемки</span><span class="sxs-lookup"><span data-stu-id="8ccd1-155">acceptances</span></span>|<span data-ttu-id="8ccd1-156">Коллекция [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="8ccd1-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="8ccd1-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-157">Read-only.</span></span> <span data-ttu-id="8ccd1-158">Сведения о принятии этого соглашения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="8ccd1-159">files</span><span class="sxs-lookup"><span data-stu-id="8ccd1-159">files</span></span>|<span data-ttu-id="8ccd1-160">[коллекция agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="8ccd1-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="8ccd1-161">PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="8ccd1-162">**Примечание:** Это свойство находится в процессе сноса.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="8ccd1-163">Вместо этого  **используйте свойство** file.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-163">Use the  **file** property instead.</span></span>|
|<span data-ttu-id="8ccd1-164">file</span><span class="sxs-lookup"><span data-stu-id="8ccd1-164">file</span></span>|[<span data-ttu-id="8ccd1-165">agreementFile</span><span class="sxs-lookup"><span data-stu-id="8ccd1-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="8ccd1-166">PDF по умолчанию, связанный с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-166">Default PDF linked to this agreement.</span></span>|
|<span data-ttu-id="8ccd1-167">файл/локализация</span><span class="sxs-lookup"><span data-stu-id="8ccd1-167">file/localizations</span></span>|<span data-ttu-id="8ccd1-168">[коллекция agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="8ccd1-168">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>|<span data-ttu-id="8ccd1-169">Локализованные версии файлов соглашений, присоединенных к соглашению.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-169">The localized versions of the agreement files attached to the agreement.</span></span>|
|<span data-ttu-id="8ccd1-170">файл/локализация/{локализацияId}/versions</span><span class="sxs-lookup"><span data-stu-id="8ccd1-170">file/localizations/{localizationId}/versions</span></span>|<span data-ttu-id="8ccd1-171">[коллекция agreementFileVersion](agreementfileversion.md)</span><span class="sxs-lookup"><span data-stu-id="8ccd1-171">[agreementFileVersion](agreementfileversion.md) collection</span></span>|<span data-ttu-id="8ccd1-172">История версий для локализованного файла соглашения.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-172">The version history for the localized agreement file.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8ccd1-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ccd1-173">JSON representation</span></span>

<span data-ttu-id="8ccd1-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ccd1-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



---
title: тип ресурса соглашения
description: Представляет настраиваемые условия соглашения об использовании клиента, созданного и управляемого с помощью Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 045d4b9142d4bd0c4bc01392975871e0253d33c0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722797"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="8d043-103">тип ресурса соглашения</span><span class="sxs-lookup"><span data-stu-id="8d043-103">agreement resource type</span></span>

<span data-ttu-id="8d043-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d043-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d043-105">Представляет настраиваемые условия соглашения об использовании клиента, созданного и управляемого с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8d043-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="8d043-106">Вы можете использовать следующие методы для создания и управления функцией [Azure Active Directory Terms of Use](/azure/active-directory/active-directory-tou) в соответствии с вашим сценарием.</span><span class="sxs-lookup"><span data-stu-id="8d043-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="8d043-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8d043-107">Methods</span></span>

| <span data-ttu-id="8d043-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8d043-108">Method</span></span>       | <span data-ttu-id="8d043-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8d043-109">Return Type</span></span> | <span data-ttu-id="8d043-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d043-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8d043-111">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="8d043-111">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="8d043-112">[коллекция соглашений](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="8d043-112">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="8d043-113">Получите коллекцию объектов соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-113">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="8d043-114">Создание соглашений</span><span class="sxs-lookup"><span data-stu-id="8d043-114">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="8d043-115">соглашение</span><span class="sxs-lookup"><span data-stu-id="8d043-115">agreement</span></span>](agreement.md) | <span data-ttu-id="8d043-116">Создайте новое соглашение, разместив в коллекции соглашений.</span><span class="sxs-lookup"><span data-stu-id="8d043-116">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="8d043-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="8d043-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="8d043-118">соглашение</span><span class="sxs-lookup"><span data-stu-id="8d043-118">agreement</span></span>](agreement.md) | <span data-ttu-id="8d043-119">Чтение свойств и связей объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="8d043-120">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="8d043-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="8d043-121">соглашение</span><span class="sxs-lookup"><span data-stu-id="8d043-121">agreement</span></span>](agreement.md) | <span data-ttu-id="8d043-122">Обновление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="8d043-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="8d043-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="8d043-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8d043-124">None</span></span> | <span data-ttu-id="8d043-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-125">Delete an agreement object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d043-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d043-126">Properties</span></span>
| <span data-ttu-id="8d043-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d043-127">Property</span></span>     | <span data-ttu-id="8d043-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8d043-128">Type</span></span>        | <span data-ttu-id="8d043-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8d043-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d043-130">displayName</span><span class="sxs-lookup"><span data-stu-id="8d043-130">displayName</span></span>|<span data-ttu-id="8d043-131">String</span><span class="sxs-lookup"><span data-stu-id="8d043-131">String</span></span>|<span data-ttu-id="8d043-132">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-132">Display name of the agreement.</span></span> <span data-ttu-id="8d043-133">Имя отображения используется для внутреннего отслеживания соглашения, но не отображается конечным пользователям, которые просматривают соглашение.</span><span class="sxs-lookup"><span data-stu-id="8d043-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="8d043-134">id</span><span class="sxs-lookup"><span data-stu-id="8d043-134">id</span></span>|<span data-ttu-id="8d043-135">String</span><span class="sxs-lookup"><span data-stu-id="8d043-135">String</span></span>| <span data-ttu-id="8d043-136">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-136">The identifier of the agreement.</span></span> <span data-ttu-id="8d043-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d043-137">Read-only.</span></span>|
|<span data-ttu-id="8d043-138">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="8d043-138">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="8d043-139">Логический</span><span class="sxs-lookup"><span data-stu-id="8d043-139">Boolean</span></span>|<span data-ttu-id="8d043-140">Указывает, должны ли конечные пользователи принимать это соглашение на каждом устройстве, с которое они имеют к нему доступ.</span><span class="sxs-lookup"><span data-stu-id="8d043-140">Indicates whether end users are required to accept this agreement on every device that they access it from.</span></span> <span data-ttu-id="8d043-141">Конечный пользователь должен зарегистрировать свое устройство в Azure AD, если он еще этого не сделал.</span><span class="sxs-lookup"><span data-stu-id="8d043-141">The end user is required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="8d043-142">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="8d043-142">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="8d043-143">Логический</span><span class="sxs-lookup"><span data-stu-id="8d043-143">Boolean</span></span>|<span data-ttu-id="8d043-144">Указывает, должен ли пользователь расширить соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="8d043-144">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="8d043-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="8d043-145">termsExpiration</span></span>|[<span data-ttu-id="8d043-146">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="8d043-146">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="8d043-147">Срок действия и периодичность соглашения для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d043-147">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="8d043-148">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="8d043-148">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="8d043-149">Duration</span><span class="sxs-lookup"><span data-stu-id="8d043-149">Duration</span></span>|<span data-ttu-id="8d043-150">Продолжительность, после которой пользователь должен повторно принять условия использования.</span><span class="sxs-lookup"><span data-stu-id="8d043-150">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="8d043-151">Значение представлено в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="8d043-151">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8d043-152">Связи</span><span class="sxs-lookup"><span data-stu-id="8d043-152">Relationships</span></span>
| <span data-ttu-id="8d043-153">Связь</span><span class="sxs-lookup"><span data-stu-id="8d043-153">Relationship</span></span> | <span data-ttu-id="8d043-154">Тип</span><span class="sxs-lookup"><span data-stu-id="8d043-154">Type</span></span>        | <span data-ttu-id="8d043-155">Описание</span><span class="sxs-lookup"><span data-stu-id="8d043-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d043-156">приемки</span><span class="sxs-lookup"><span data-stu-id="8d043-156">acceptances</span></span>|<span data-ttu-id="8d043-157">Коллекция [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="8d043-157">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="8d043-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d043-158">Read-only.</span></span> <span data-ttu-id="8d043-159">Сведения о принятии этого соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-159">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="8d043-160">files</span><span class="sxs-lookup"><span data-stu-id="8d043-160">files</span></span>|<span data-ttu-id="8d043-161">[коллекция agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="8d043-161">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="8d043-162">PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="8d043-162">PDFs linked to this agreement.</span></span> <span data-ttu-id="8d043-163">Это свойство находится в процессе сноса.</span><span class="sxs-lookup"><span data-stu-id="8d043-163">This property is in the process of being deprecated.</span></span> <span data-ttu-id="8d043-164">Вместо этого  **используйте свойство** file.</span><span class="sxs-lookup"><span data-stu-id="8d043-164">Use the  **file** property instead.</span></span>|
|<span data-ttu-id="8d043-165">file</span><span class="sxs-lookup"><span data-stu-id="8d043-165">file</span></span>|[<span data-ttu-id="8d043-166">agreementFile</span><span class="sxs-lookup"><span data-stu-id="8d043-166">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="8d043-167">PDF по умолчанию, связанный с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="8d043-167">Default PDF linked to this agreement.</span></span>|
|<span data-ttu-id="8d043-168">локализация</span><span class="sxs-lookup"><span data-stu-id="8d043-168">localizations</span></span>|<span data-ttu-id="8d043-169">[коллекция agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="8d043-169">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>|<span data-ttu-id="8d043-170">Локализованные версии файлов соглашений, присоединенных к соглашению.</span><span class="sxs-lookup"><span data-stu-id="8d043-170">The localized versions of the agreement files attached to the agreement.</span></span>|
|<span data-ttu-id="8d043-171">versions</span><span class="sxs-lookup"><span data-stu-id="8d043-171">versions</span></span>|<span data-ttu-id="8d043-172">[коллекция agreementFileVersion](agreementfileversion.md)</span><span class="sxs-lookup"><span data-stu-id="8d043-172">[agreementFileVersion](agreementfileversion.md) collection</span></span>|<span data-ttu-id="8d043-173">История версий для локализованного файла соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d043-173">The version history for the localized agreement file.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8d043-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d043-174">JSON representation</span></span>

<span data-ttu-id="8d043-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d043-175">The following is a JSON representation of the resource.</span></span>

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



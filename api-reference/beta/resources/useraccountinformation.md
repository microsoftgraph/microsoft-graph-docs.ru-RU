---
title: Тип ресурса Усераккаунтинформатион
description: Тип ресурса Усераккаунтинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a633b6de9269b67fcf26dea035438a3494c4515c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812746"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="e9f2e-103">Тип ресурса Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-103">userAccountInformation resource type</span></span>

<span data-ttu-id="e9f2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9f2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f2e-105">Представляет сведения, специально связанные с учетной записью пользователя, будь то учетная запись Azure AD или учетная запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-105">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="e9f2e-106">Идентификатор сущности задается соответствующим идентификаторам Azure AD AD или CID учетной записи Майкрософт соответственно.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-106">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="e9f2e-107">Эти поля доступны только для чтения через Microsoft Graph и должны редактироваться с помощью профиля пользователя или администратора клиента для соответствующего интерфейса.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-107">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="e9f2e-108">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-108">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e9f2e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e9f2e-109">Methods</span></span>

|<span data-ttu-id="e9f2e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e9f2e-110">Method</span></span>|<span data-ttu-id="e9f2e-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e9f2e-111">Return type</span></span>|<span data-ttu-id="e9f2e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e9f2e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9f2e-113">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="e9f2e-113">List accounts</span></span>](../api/profile-list-accounts.md)|<span data-ttu-id="e9f2e-114">Коллекция [усераккаунтинформатион](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="e9f2e-114">[userAccountInformation](../resources/useraccountinformation.md) collection</span></span>|<span data-ttu-id="e9f2e-115">Получение ресурсов Усераккаунтинформатион из свойства навигации учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-115">Get the userAccountInformation resources from the account navigation property.</span></span>|
|[<span data-ttu-id="e9f2e-116">Создание Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-116">Create userAccountInformation</span></span>](../api/profile-post-accounts.md)|[<span data-ttu-id="e9f2e-117">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-117">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="e9f2e-118">Создание нового объекта Усераккаунтинформатион.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-118">Create a new userAccountInformation object.</span></span>|
|[<span data-ttu-id="e9f2e-119">Получение Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-119">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md)|[<span data-ttu-id="e9f2e-120">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-120">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="e9f2e-121">Чтение свойств и связей объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="e9f2e-121">Read the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="e9f2e-122">Обновление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-122">Update userAccountInformation</span></span>](../api/useraccountinformation-update.md)|[<span data-ttu-id="e9f2e-123">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-123">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="e9f2e-124">Обновление свойств объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="e9f2e-124">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="e9f2e-125">Удаление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="e9f2e-125">Delete userAccountInformation</span></span>](../api/useraccountinformation-delete.md)|<span data-ttu-id="e9f2e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e9f2e-126">None</span></span>|<span data-ttu-id="e9f2e-127">Удаляет объект [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="e9f2e-127">Deletes a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e9f2e-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9f2e-128">Properties</span></span>

|<span data-ttu-id="e9f2e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9f2e-129">Property</span></span>|<span data-ttu-id="e9f2e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e9f2e-130">Type</span></span>|<span data-ttu-id="e9f2e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e9f2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f2e-132">ageGroup</span><span class="sxs-lookup"><span data-stu-id="e9f2e-132">ageGroup</span></span>|<span data-ttu-id="e9f2e-133">String</span><span class="sxs-lookup"><span data-stu-id="e9f2e-133">String</span></span>|<span data-ttu-id="e9f2e-134">Показывает группу возрастных пользователей.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-134">Shows the age group of user.</span></span> <span data-ttu-id="e9f2e-135">Допустимые `null` значения `minor` , `notAdult` и `adult` они создаются каталогом и не могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-135">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="e9f2e-136">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="e9f2e-136">allowedAudiences</span></span>|<span data-ttu-id="e9f2e-137">String</span><span class="sxs-lookup"><span data-stu-id="e9f2e-137">String</span></span>|<span data-ttu-id="e9f2e-138">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e9f2e-139">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e9f2e-140">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e9f2e-141">countryCode</span><span class="sxs-lookup"><span data-stu-id="e9f2e-141">countryCode</span></span>|<span data-ttu-id="e9f2e-142">String</span><span class="sxs-lookup"><span data-stu-id="e9f2e-142">String</span></span>|<span data-ttu-id="e9f2e-143">Содержит двухбуквенный код страны, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-143">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="e9f2e-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="e9f2e-144">createdBy</span></span>|[<span data-ttu-id="e9f2e-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9f2e-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="e9f2e-146">Предоставляет идентификатор пользователя и/или приложения, создавшего сущность.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-146">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="e9f2e-147">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e9f2e-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9f2e-148">createdDateTime</span></span>|<span data-ttu-id="e9f2e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9f2e-149">DateTimeOffset</span></span>|<span data-ttu-id="e9f2e-150">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-150">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="e9f2e-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e9f2e-152">id</span><span class="sxs-lookup"><span data-stu-id="e9f2e-152">id</span></span>|<span data-ttu-id="e9f2e-153">String</span><span class="sxs-lookup"><span data-stu-id="e9f2e-153">String</span></span>|<span data-ttu-id="e9f2e-154">Идентификатор, используемый для индивидуальной адресации объекта.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="e9f2e-155">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="e9f2e-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="e9f2e-156">выводов</span><span class="sxs-lookup"><span data-stu-id="e9f2e-156">inference</span></span>|[<span data-ttu-id="e9f2e-157">инференцедата</span><span class="sxs-lookup"><span data-stu-id="e9f2e-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e9f2e-158">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e9f2e-159">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e9f2e-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e9f2e-160">lastModifiedBy</span></span>|[<span data-ttu-id="e9f2e-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9f2e-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="e9f2e-162">Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="e9f2e-163">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e9f2e-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9f2e-164">lastModifiedDateTime</span></span>|<span data-ttu-id="e9f2e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9f2e-165">DateTimeOffset</span></span>|<span data-ttu-id="e9f2e-166">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="e9f2e-167">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e9f2e-168">преферредлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="e9f2e-168">preferredLanguageTag</span></span>|[<span data-ttu-id="e9f2e-169">localeInfo</span><span class="sxs-lookup"><span data-stu-id="e9f2e-169">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="e9f2e-170">Содержит язык, который пользователь связал с учетной записью как предпочитаемый.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-170">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="e9f2e-171">source</span><span class="sxs-lookup"><span data-stu-id="e9f2e-171">source</span></span>|[<span data-ttu-id="e9f2e-172">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="e9f2e-172">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="e9f2e-173">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-173">Where the values originated if synced from another service.</span></span> <span data-ttu-id="e9f2e-174">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9f2e-174">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e9f2e-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9f2e-175">userPrincipalName</span></span>|<span data-ttu-id="e9f2e-176">String</span><span class="sxs-lookup"><span data-stu-id="e9f2e-176">String</span></span>|<span data-ttu-id="e9f2e-177">Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-177">The user principal name (UPN) of the user associated with the account.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="e9f2e-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="e9f2e-178">Relationships</span></span>
<span data-ttu-id="e9f2e-179">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9f2e-180">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e9f2e-180">JSON representation</span></span>
<span data-ttu-id="e9f2e-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9f2e-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```

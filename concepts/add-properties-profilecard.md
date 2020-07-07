---
title: Настройка карточки профиля с помощью API профилей в Microsoft Graph (Предварительная версия)
description: В этой статье описывается, как можно настроить карточку профиля, сделав дополнительные атрибуты видимыми, или добавить настраиваемые атрибуты.
author: PollyNincevic
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: dc0c78ecfdf00488c7c9c12969eea8b405be496c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050979"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-api-in-microsoft-graph-preview"></a><span data-ttu-id="3c0be-103">Добавление дополнительных свойств в карточку профиля с помощью API профилей в Microsoft Graph (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3c0be-103">Add additional properties to the profile card using the profile API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="3c0be-104">В [карточке профиля](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) в Microsoft 365 можно найти сведения о пользователях, которые хранятся и поддерживаются организацией, например **названием должности** или **местоположением офиса**.</span><span class="sxs-lookup"><span data-stu-id="3c0be-104">On the [profile card](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) in Microsoft 365, you can find information about users that is stored and maintained by your organization, for example **Job title** or **Office location**.</span></span>

<span data-ttu-id="3c0be-105">Используйте ресурс [профилекардпроперти](/graph/api/resources/profilecardproperty?view=graph-rest-beta) для отображения дополнительных свойств из Azure AD в карточках профилей для Организации, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="3c0be-105">Use the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource to show additional properties from Azure AD on profile cards for an organization, by:</span></span>

- <span data-ttu-id="3c0be-106">Отображение дополнительных атрибутов</span><span class="sxs-lookup"><span data-stu-id="3c0be-106">Making additional attributes visible</span></span>

- <span data-ttu-id="3c0be-107">Добавление настраиваемых атрибутов</span><span class="sxs-lookup"><span data-stu-id="3c0be-107">Adding custom attributes</span></span>

<span data-ttu-id="3c0be-108">Дополнительные свойства будут отображаться в разделе **контакт** карточки профиля в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3c0be-108">Additional properties will display in the **Contact** section of the profile card in Microsoft 365.</span></span>

> [!NOTE]
><span data-ttu-id="3c0be-109">Для выполнения операций над ресурсом **профилекардпроперти** , использующим делегированные разрешения, необходимо, чтобы вошедшего в систему пользователя была назначена роль "Администратор клиента" или "Глобальный администратор".</span><span class="sxs-lookup"><span data-stu-id="3c0be-109">Operations on the **profileCardProperty** resource that use delegated permissions requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="make-additional-attributes-visible"></a><span data-ttu-id="3c0be-110">Сделать дополнительные атрибуты видимыми</span><span class="sxs-lookup"><span data-stu-id="3c0be-110">Make additional attributes visible</span></span>

<span data-ttu-id="3c0be-111">Вы можете сделать следующие атрибуты из Azure Active Directory (Azure AD) видимыми в карточках профилей пользователей.</span><span class="sxs-lookup"><span data-stu-id="3c0be-111">You can make the following attributes from Azure Active Directory (Azure AD) visible on users' profile cards.</span></span> <span data-ttu-id="3c0be-112">В этих атрибутах *не учитывается регистр*:</span><span class="sxs-lookup"><span data-stu-id="3c0be-112">These attributes are *not case-sensitive*:</span></span>

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

<span data-ttu-id="3c0be-113">В следующей таблице показано, как атрибуты Azure AD соответствуют свойствам объекта [пользователя](/graph/api/resources/user?view=graph-rest-beta) Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3c0be-113">The following table shows how the Azure AD attributes correspond with properties of the Microsoft Graph [user](/graph/api/resources/user?view=graph-rest-beta) entity.</span></span>

|<span data-ttu-id="3c0be-114">Атрибут Azure AD</span><span class="sxs-lookup"><span data-stu-id="3c0be-114">Azure AD attribute</span></span> |<span data-ttu-id="3c0be-115">Свойство сущности пользователя</span><span class="sxs-lookup"><span data-stu-id="3c0be-115">User entity property</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3c0be-116">UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3c0be-116">UserPrincipalName</span></span>|<span data-ttu-id="3c0be-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3c0be-117">userPrincipalName</span></span> |
|<span data-ttu-id="3c0be-118">Факс</span><span class="sxs-lookup"><span data-stu-id="3c0be-118">Fax</span></span>|<span data-ttu-id="3c0be-119">faxNumber</span><span class="sxs-lookup"><span data-stu-id="3c0be-119">faxNumber</span></span>|
|<span data-ttu-id="3c0be-120">StreetAddress</span><span class="sxs-lookup"><span data-stu-id="3c0be-120">StreetAddress</span></span>|<span data-ttu-id="3c0be-121">streetAddress</span><span class="sxs-lookup"><span data-stu-id="3c0be-121">streetAddress</span></span>|
|<span data-ttu-id="3c0be-122">PostalCode</span><span class="sxs-lookup"><span data-stu-id="3c0be-122">PostalCode</span></span>|<span data-ttu-id="3c0be-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="3c0be-123">postalCode</span></span>|
|<span data-ttu-id="3c0be-124">StateOrProvince</span><span class="sxs-lookup"><span data-stu-id="3c0be-124">StateOrProvince</span></span>|<span data-ttu-id="3c0be-125">состояние</span><span class="sxs-lookup"><span data-stu-id="3c0be-125">state</span></span>
|<span data-ttu-id="3c0be-126">Alias</span><span class="sxs-lookup"><span data-stu-id="3c0be-126">Alias</span></span>|<span data-ttu-id="3c0be-127">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3c0be-127">mailNickname</span></span>

<span data-ttu-id="3c0be-128">Вы можете добавить любой из этих атрибутов в карточку профиля, настроив [Параметры организации](/graph/api/resources/organizationsettings?view=graph-rest-beta) и добавив атрибут в качестве свойства *Директорипропертинаме*\* объекта **профилекардпроперти** в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3c0be-128">You can add any of these attributes to the profile card by configuring your [organization settings](/graph/api/resources/organizationsettings?view=graph-rest-beta) and adding the attribute as the *directoryPropertyName*\* property of a **profileCardProperty** in Microsoft Graph.</span></span> <span data-ttu-id="3c0be-129">Когда вы сделаете дополнительные атрибуты видимыми, необходимо использовать имена свойств для `en-us` .</span><span class="sxs-lookup"><span data-stu-id="3c0be-129">When you make additional attributes visible, you must use the property names for `en-us`.</span></span> <span data-ttu-id="3c0be-130">Вам не нужно добавлять локализованные значения.</span><span class="sxs-lookup"><span data-stu-id="3c0be-130">You don't have to add localized values.</span></span> <span data-ttu-id="3c0be-131">Дополнительные свойства будут автоматически отображаться в языковых параметрах, заданных пользователем для Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3c0be-131">The additional properties will automatically be shown in the language settings that the user has specified for Microsoft 365.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3c0be-132">При добавлении атрибута в карточку профиля для отображения добавления потребуется до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="3c0be-132">When adding an attribute to profile card, it takes up to 24 hours for the addition to be displayed.</span></span>

## <a name="example"></a><span data-ttu-id="3c0be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3c0be-133">Example</span></span>

<span data-ttu-id="3c0be-134">В приведенном ниже примере показано, как отобразить `Alias` атрибут в карточке профиля:</span><span class="sxs-lookup"><span data-stu-id="3c0be-134">The following example displays the `Alias` attribute on the profile card:</span></span>

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

<span data-ttu-id="3c0be-135">В случае успеха ответ возвращает `201 OK` код отклика и объект **профилекардпроперти** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c0be-135">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="3c0be-136">Значение `Alias` атрибута будет отображаться на карточке профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c0be-136">The value for the `Alias` attribute  would be displayed on a user's profile card.</span></span>  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a><span data-ttu-id="3c0be-137">Добавление настраиваемых атрибутов</span><span class="sxs-lookup"><span data-stu-id="3c0be-137">Adding custom attributes</span></span>

<span data-ttu-id="3c0be-138">Вы можете добавить в карты профилей пользователей любое из 15 [настраиваемых атрибутов настраиваемого расширения](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) Azure AD, настроив параметры организации и [добавив соответствующее значение в качестве Профилекардпроперти](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3c0be-138">You can add any of the 15 Azure AD [custom extension attributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) to users' profile cards by configuring your organization settings and [adding the corresponding value as a profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) in Microsoft Graph.</span></span> <span data-ttu-id="3c0be-139">Можно добавить один ресурс **профилекардпроперти** за раз.</span><span class="sxs-lookup"><span data-stu-id="3c0be-139">You can add one **profileCardProperty** resource at a time.</span></span>

<span data-ttu-id="3c0be-140">Изменения, отображаемые в карточках профилей, занимают до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="3c0be-140">It takes up to 24 hours for the changes to show on profile cards.</span></span>

<span data-ttu-id="3c0be-141">Настраиваемые свойства не поддерживают поиск и не могут использоваться для поиска людей в приложениях и службах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3c0be-141">Custom properties are not searchable and can't be used to search for people across Microsoft apps and services.</span></span>

<span data-ttu-id="3c0be-142">В следующей таблице показано, как имена настраиваемых атрибутов расширения Azure AD соответствуют поддерживаемым значениям для свойства **директорипропертинаме** ресурса [профилекардпроперти](/graph/api/resources/profilecardproperty?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="3c0be-142">The following table shows how the Azure AD custom extension attribute names correspond to the supported values for the **directoryPropertyName** property of the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource.</span></span> <span data-ttu-id="3c0be-143">В именах настраиваемых атрибутов настраиваемого расширения Azure AD *не учитывается регистр*:</span><span class="sxs-lookup"><span data-stu-id="3c0be-143">These Azure AD custom extension attribute names are *not case-sensitive*:</span></span>

|<span data-ttu-id="3c0be-144">Настраиваемый атрибут расширения Azure AD</span><span class="sxs-lookup"><span data-stu-id="3c0be-144">Azure AD custom extension attribute</span></span> | <span data-ttu-id="3c0be-145">Значение для указания в качестве Директорипропертинаме</span><span class="sxs-lookup"><span data-stu-id="3c0be-145">Value to specify as directoryPropertyName</span></span> |
|:--------------------|:-----------------|
| <span data-ttu-id="3c0be-146">От extensionattribute1</span><span class="sxs-lookup"><span data-stu-id="3c0be-146">extensionAttribute1</span></span> | <span data-ttu-id="3c0be-147">customAttribute1</span><span class="sxs-lookup"><span data-stu-id="3c0be-147">customAttribute1</span></span> |
| <span data-ttu-id="3c0be-148">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="3c0be-148">extensionAttribute2</span></span> | <span data-ttu-id="3c0be-149">customAttribute2</span><span class="sxs-lookup"><span data-stu-id="3c0be-149">customAttribute2</span></span> |
| <span data-ttu-id="3c0be-150">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="3c0be-150">extensionAttribute3</span></span> | <span data-ttu-id="3c0be-151">customAttribute3</span><span class="sxs-lookup"><span data-stu-id="3c0be-151">customAttribute3</span></span> |
| <span data-ttu-id="3c0be-152">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="3c0be-152">extensionAttribute4</span></span> | <span data-ttu-id="3c0be-153">customAttribute4</span><span class="sxs-lookup"><span data-stu-id="3c0be-153">customAttribute4</span></span> |
| <span data-ttu-id="3c0be-154">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="3c0be-154">extensionAttribute5</span></span> | <span data-ttu-id="3c0be-155">customAttribute5</span><span class="sxs-lookup"><span data-stu-id="3c0be-155">customAttribute5</span></span> |
| <span data-ttu-id="3c0be-156">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="3c0be-156">extensionAttribute6</span></span> | <span data-ttu-id="3c0be-157">customAttribute6</span><span class="sxs-lookup"><span data-stu-id="3c0be-157">customAttribute6</span></span> |
| <span data-ttu-id="3c0be-158">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="3c0be-158">extensionAttribute7</span></span> | <span data-ttu-id="3c0be-159">customAttribute7</span><span class="sxs-lookup"><span data-stu-id="3c0be-159">customAttribute7</span></span> |
| <span data-ttu-id="3c0be-160">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="3c0be-160">extensionAttribute8</span></span> | <span data-ttu-id="3c0be-161">customAttribute8</span><span class="sxs-lookup"><span data-stu-id="3c0be-161">customAttribute8</span></span> |
| <span data-ttu-id="3c0be-162">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="3c0be-162">extensionAttribute9</span></span> | <span data-ttu-id="3c0be-163">customAttribute9</span><span class="sxs-lookup"><span data-stu-id="3c0be-163">customAttribute9</span></span> |
| <span data-ttu-id="3c0be-164">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="3c0be-164">extensionAttribute10</span></span> | <span data-ttu-id="3c0be-165">customAttribute10</span><span class="sxs-lookup"><span data-stu-id="3c0be-165">customAttribute10</span></span> |
| <span data-ttu-id="3c0be-166">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="3c0be-166">extensionAttribute11</span></span> | <span data-ttu-id="3c0be-167">customAttribute11</span><span class="sxs-lookup"><span data-stu-id="3c0be-167">customAttribute11</span></span> |
| <span data-ttu-id="3c0be-168">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="3c0be-168">extensionAttribute12</span></span> | <span data-ttu-id="3c0be-169">customAttribute12</span><span class="sxs-lookup"><span data-stu-id="3c0be-169">customAttribute12</span></span> |
| <span data-ttu-id="3c0be-170">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="3c0be-170">extensionAttribute13</span></span> | <span data-ttu-id="3c0be-171">customAttribute13</span><span class="sxs-lookup"><span data-stu-id="3c0be-171">customAttribute13</span></span> |
| <span data-ttu-id="3c0be-172">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="3c0be-172">extensionAttribute14</span></span> | <span data-ttu-id="3c0be-173">customAttribute14</span><span class="sxs-lookup"><span data-stu-id="3c0be-173">customAttribute14</span></span> |
| <span data-ttu-id="3c0be-174">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="3c0be-174">extensionAttribute15</span></span> | <span data-ttu-id="3c0be-175">customAttribute15</span><span class="sxs-lookup"><span data-stu-id="3c0be-175">customAttribute15</span></span> |

## <a name="example"></a><span data-ttu-id="3c0be-176">Пример</span><span class="sxs-lookup"><span data-stu-id="3c0be-176">Example</span></span>

<span data-ttu-id="3c0be-177">В следующем примере первый атрибут настраиваемого расширения Azure AD добавляется в карточку профиля с использованием отображаемого имени **центра затрат**.</span><span class="sxs-lookup"><span data-stu-id="3c0be-177">The following example adds the first Azure AD custom extension attribute to the profile card, using the display name **Cost center**.</span></span> <span data-ttu-id="3c0be-178">Для пользователей, для которых в качестве языковых параметров задан немецкий, отображаемое имя будет **костенстелле**.</span><span class="sxs-lookup"><span data-stu-id="3c0be-178">For users that have set their language settings to German, the display name will be **Kostenstelle**.</span></span>

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

<span data-ttu-id="3c0be-179">Если язык не поддерживается, будет отображаться имя свойства со значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c0be-179">If a language is not supported, the property name will be shown with the default value.</span></span>  

<span data-ttu-id="3c0be-180">В случае успеха ответ возвращает `201 OK` код отклика и объект **профилекардпроперти** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c0be-180">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="3c0be-181">В этом примере можно предположить, что в карточке профиля отображается **костенстелле** для всех пользователей, для которых в карточке профиля задан немецкий языковой параметр.</span><span class="sxs-lookup"><span data-stu-id="3c0be-181">In this example you can assume that the profile card displays **Kostenstelle** for all users that have set their language settings to German on the profile card.</span></span> <span data-ttu-id="3c0be-182">Для всех остальных пользователей **центр затрат** будет отображаться в карточке профиля.</span><span class="sxs-lookup"><span data-stu-id="3c0be-182">For all other users, **Cost center** will be displayed on the profile card.</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="3c0be-183">См. также</span><span class="sxs-lookup"><span data-stu-id="3c0be-183">See also</span></span>

[<span data-ttu-id="3c0be-184">Поиск идентификатора клиента Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3c0be-184">Find your Microsoft 365 tenant ID</span></span>](https://docs.microsoft.com/onedrive/find-your-office-365-tenant-id)

[<span data-ttu-id="3c0be-185">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="3c0be-185">onPremisesExtensionAttributes resource type</span></span>](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[<span data-ttu-id="3c0be-186">Тип ресурса "пользователь"</span><span class="sxs-lookup"><span data-stu-id="3c0be-186">User resource type</span></span>](/graph/api/resources/user?view=graph-rest-beta)

[<span data-ttu-id="3c0be-187">Проводник графиков</span><span class="sxs-lookup"><span data-stu-id="3c0be-187">Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)

[<span data-ttu-id="3c0be-188">Получение Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="3c0be-188">Get profileCardProperty</span></span>](/graph/api/profilecardproperty-get?view=graph-rest-beta)

---
title: Настройка карточки профиля с помощью API профиля в Microsoft Graph (предварительная версия)
description: В этой статье описано, как настроить карточку профиля, сделав видимыми дополнительные атрибуты или добавив настраиваемые атрибуты.
author: PollyNincevic
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5df48bc8da848c6e5655467ad9ef39a8bb992026
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288786"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a><span data-ttu-id="1c883-103">Добавление свойств в карточку профиля с помощью API карточки профиля в Microsoft Graph (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c883-103">Add additional properties to the profile card using the profile card API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="1c883-104">На [карточке профиля](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) в Microsoft 365 находится информация о пользователях, сохраненная и управляемая вашей организацией, например **Должность** или **Местонахождение офиса**.</span><span class="sxs-lookup"><span data-stu-id="1c883-104">On the [profile card](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) in Microsoft 365, you can find information about users that is stored and maintained by your organization, for example **Job title** or **Office location**.</span></span>

<span data-ttu-id="1c883-105">Используйте ресурс [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta), чтобы отображать дополнительные свойства из Azure AD в карточках профилей для организации следующим образом:</span><span class="sxs-lookup"><span data-stu-id="1c883-105">Use the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource to show additional properties from Azure AD on profile cards for an organization, by:</span></span>

- <span data-ttu-id="1c883-106">Обеспечение видимости дополнительных атрибутов</span><span class="sxs-lookup"><span data-stu-id="1c883-106">Making additional attributes visible</span></span>

- <span data-ttu-id="1c883-107">Добавление настраиваемых атрибутов</span><span class="sxs-lookup"><span data-stu-id="1c883-107">Adding custom attributes</span></span>

<span data-ttu-id="1c883-108">Дополнительные свойства отображаются в разделе **Контакт** карточки профиля в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1c883-108">Additional properties will display in the **Contact** section of the profile card in Microsoft 365.</span></span>

> [!NOTE]
><span data-ttu-id="1c883-109">Операции в ресурсе **profileCardProperty**, использующем делегированные разрешения, требуют, чтобы у вошедшего пользователя была роль администратора клиента или глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="1c883-109">Operations on the **profileCardProperty** resource that use delegated permissions requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="make-additional-attributes-visible"></a><span data-ttu-id="1c883-110">Обеспечение видимости дополнительных атрибутов</span><span class="sxs-lookup"><span data-stu-id="1c883-110">Make additional attributes visible</span></span>

<span data-ttu-id="1c883-111">Вы можете сделать видимыми в карточках профилей пользователей следующие атрибуты из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1c883-111">You can make the following attributes from Azure Active Directory (Azure AD) visible on users' profile cards.</span></span> <span data-ttu-id="1c883-112">В этих атрибутах *регистр не учитывается*:</span><span class="sxs-lookup"><span data-stu-id="1c883-112">These attributes are *not case-sensitive*:</span></span>

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

<span data-ttu-id="1c883-113">В таблице ниже показано соответствие атрибутов Azure AD свойствам объекта [user](/graph/api/resources/user?view=graph-rest-beta) Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c883-113">The following table shows how the Azure AD attributes correspond with properties of the Microsoft Graph [user](/graph/api/resources/user?view=graph-rest-beta) entity.</span></span>

|<span data-ttu-id="1c883-114">Атрибут Azure AD</span><span class="sxs-lookup"><span data-stu-id="1c883-114">Azure AD attribute</span></span> |<span data-ttu-id="1c883-115">Свойство объекта user</span><span class="sxs-lookup"><span data-stu-id="1c883-115">User entity property</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1c883-116">UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1c883-116">UserPrincipalName</span></span>|<span data-ttu-id="1c883-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1c883-117">userPrincipalName</span></span> |
|<span data-ttu-id="1c883-118">Fax</span><span class="sxs-lookup"><span data-stu-id="1c883-118">Fax</span></span>|<span data-ttu-id="1c883-119">faxNumber</span><span class="sxs-lookup"><span data-stu-id="1c883-119">faxNumber</span></span>|
|<span data-ttu-id="1c883-120">StreetAddress</span><span class="sxs-lookup"><span data-stu-id="1c883-120">StreetAddress</span></span>|<span data-ttu-id="1c883-121">streetAddress</span><span class="sxs-lookup"><span data-stu-id="1c883-121">streetAddress</span></span>|
|<span data-ttu-id="1c883-122">PostalCode</span><span class="sxs-lookup"><span data-stu-id="1c883-122">PostalCode</span></span>|<span data-ttu-id="1c883-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="1c883-123">postalCode</span></span>|
|<span data-ttu-id="1c883-124">StateOrProvince</span><span class="sxs-lookup"><span data-stu-id="1c883-124">StateOrProvince</span></span>|<span data-ttu-id="1c883-125">state</span><span class="sxs-lookup"><span data-stu-id="1c883-125">state</span></span>
|<span data-ttu-id="1c883-126">Alias</span><span class="sxs-lookup"><span data-stu-id="1c883-126">Alias</span></span>|<span data-ttu-id="1c883-127">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1c883-127">mailNickname</span></span>

<span data-ttu-id="1c883-128">Вы можете добавить любой из этих атрибутов в карточку профиля, настроив [параметры организации](/graph/api/resources/organizationsettings?view=graph-rest-beta) и добавив его в качестве свойства *directoryPropertyName*\* ресурса **profileCardProperty** в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c883-128">You can add any of these attributes to the profile card by configuring your [organization settings](/graph/api/resources/organizationsettings?view=graph-rest-beta) and adding the attribute as the *directoryPropertyName*\* property of a **profileCardProperty** in Microsoft Graph.</span></span> <span data-ttu-id="1c883-129">Когда вы делаете дополнительные атрибуты видимыми, вы должны использовать имена свойств в формате `en-us`.</span><span class="sxs-lookup"><span data-stu-id="1c883-129">When you make additional attributes visible, you must use the property names for `en-us`.</span></span> <span data-ttu-id="1c883-130">Вам не требуется добавлять локализованные значения.</span><span class="sxs-lookup"><span data-stu-id="1c883-130">You don't have to add localized values.</span></span> <span data-ttu-id="1c883-131">Дополнительные свойства будут автоматически отображаться с использованием языковых настроек, указанных пользователем в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1c883-131">The additional properties will automatically be shown in the language settings that the user has specified for Microsoft 365.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1c883-132">При добавлении атрибута в карточку профиля его отображение занимает до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="1c883-132">When adding an attribute to profile card, it takes up to 24 hours for the addition to be displayed.</span></span>

## <a name="example"></a><span data-ttu-id="1c883-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1c883-133">Example</span></span>

<span data-ttu-id="1c883-134">В следующем примере в карточке профиля отображается атрибут `Alias`:</span><span class="sxs-lookup"><span data-stu-id="1c883-134">The following example displays the `Alias` attribute on the profile card:</span></span>

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

<span data-ttu-id="1c883-135">При успешном выполнении возвращается код отклика `201 OK` и объект **profileCardProperty** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c883-135">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="1c883-136">Значение атрибута `Alias` отображается в карточке профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c883-136">The value for the `Alias` attribute  would be displayed on a user's profile card.</span></span>  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a><span data-ttu-id="1c883-137">Добавление настраиваемых атрибутов</span><span class="sxs-lookup"><span data-stu-id="1c883-137">Adding custom attributes</span></span>

<span data-ttu-id="1c883-138">Вы можете добавлять в карточки профилей пользователей любой из 15 [настраиваемых атрибутов расширений](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) Azure AD путем настройки параметров организации и [добавления соответствующего значения в качестве profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c883-138">You can add any of the 15 Azure AD [custom extension attributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) to users' profile cards by configuring your organization settings and [adding the corresponding value as a profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) in Microsoft Graph.</span></span> <span data-ttu-id="1c883-139">Вы можете добавить один ресурс **profileCardProperty** за один раз.</span><span class="sxs-lookup"><span data-stu-id="1c883-139">You can add one **profileCardProperty** resource at a time.</span></span>

<span data-ttu-id="1c883-140">Отображение внесенных изменений в карточках профилей занимают до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="1c883-140">It takes up to 24 hours for the changes to show on profile cards.</span></span>

<span data-ttu-id="1c883-141">Настраиваемые свойства не поддерживают поиск, и их невозможно использовать для поиска людей в различных приложениях и службах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1c883-141">Custom properties are not searchable and can't be used to search for people across Microsoft apps and services.</span></span>

<span data-ttu-id="1c883-142">В таблице ниже показано, как имена настраиваемых атрибутов расширений Azure AD соответствуют поддерживаемым значениям свойства **directoryPropertyName** ресурса [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="1c883-142">The following table shows how the Azure AD custom extension attribute names correspond to the supported values for the **directoryPropertyName** property of the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource.</span></span> <span data-ttu-id="1c883-143">В именах настраиваемых атрибутов расширений Azure AD *регистр не учитывается*:</span><span class="sxs-lookup"><span data-stu-id="1c883-143">These Azure AD custom extension attribute names are *not case-sensitive*:</span></span>

|<span data-ttu-id="1c883-144">Настраиваемый атрибут расширения Azure AD</span><span class="sxs-lookup"><span data-stu-id="1c883-144">Azure AD custom extension attribute</span></span> | <span data-ttu-id="1c883-145">Значение, указываемое в качестве directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="1c883-145">Value to specify as directoryPropertyName</span></span> |
|:--------------------|:-----------------|
| <span data-ttu-id="1c883-146">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="1c883-146">extensionAttribute1</span></span> | <span data-ttu-id="1c883-147">customAttribute1</span><span class="sxs-lookup"><span data-stu-id="1c883-147">customAttribute1</span></span> |
| <span data-ttu-id="1c883-148">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="1c883-148">extensionAttribute2</span></span> | <span data-ttu-id="1c883-149">customAttribute2</span><span class="sxs-lookup"><span data-stu-id="1c883-149">customAttribute2</span></span> |
| <span data-ttu-id="1c883-150">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="1c883-150">extensionAttribute3</span></span> | <span data-ttu-id="1c883-151">customAttribute3</span><span class="sxs-lookup"><span data-stu-id="1c883-151">customAttribute3</span></span> |
| <span data-ttu-id="1c883-152">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="1c883-152">extensionAttribute4</span></span> | <span data-ttu-id="1c883-153">customAttribute4</span><span class="sxs-lookup"><span data-stu-id="1c883-153">customAttribute4</span></span> |
| <span data-ttu-id="1c883-154">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="1c883-154">extensionAttribute5</span></span> | <span data-ttu-id="1c883-155">customAttribute5</span><span class="sxs-lookup"><span data-stu-id="1c883-155">customAttribute5</span></span> |
| <span data-ttu-id="1c883-156">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="1c883-156">extensionAttribute6</span></span> | <span data-ttu-id="1c883-157">customAttribute6</span><span class="sxs-lookup"><span data-stu-id="1c883-157">customAttribute6</span></span> |
| <span data-ttu-id="1c883-158">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="1c883-158">extensionAttribute7</span></span> | <span data-ttu-id="1c883-159">customAttribute7</span><span class="sxs-lookup"><span data-stu-id="1c883-159">customAttribute7</span></span> |
| <span data-ttu-id="1c883-160">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="1c883-160">extensionAttribute8</span></span> | <span data-ttu-id="1c883-161">customAttribute8</span><span class="sxs-lookup"><span data-stu-id="1c883-161">customAttribute8</span></span> |
| <span data-ttu-id="1c883-162">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="1c883-162">extensionAttribute9</span></span> | <span data-ttu-id="1c883-163">customAttribute9</span><span class="sxs-lookup"><span data-stu-id="1c883-163">customAttribute9</span></span> |
| <span data-ttu-id="1c883-164">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="1c883-164">extensionAttribute10</span></span> | <span data-ttu-id="1c883-165">customAttribute10</span><span class="sxs-lookup"><span data-stu-id="1c883-165">customAttribute10</span></span> |
| <span data-ttu-id="1c883-166">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="1c883-166">extensionAttribute11</span></span> | <span data-ttu-id="1c883-167">customAttribute11</span><span class="sxs-lookup"><span data-stu-id="1c883-167">customAttribute11</span></span> |
| <span data-ttu-id="1c883-168">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="1c883-168">extensionAttribute12</span></span> | <span data-ttu-id="1c883-169">customAttribute12</span><span class="sxs-lookup"><span data-stu-id="1c883-169">customAttribute12</span></span> |
| <span data-ttu-id="1c883-170">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="1c883-170">extensionAttribute13</span></span> | <span data-ttu-id="1c883-171">customAttribute13</span><span class="sxs-lookup"><span data-stu-id="1c883-171">customAttribute13</span></span> |
| <span data-ttu-id="1c883-172">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="1c883-172">extensionAttribute14</span></span> | <span data-ttu-id="1c883-173">customAttribute14</span><span class="sxs-lookup"><span data-stu-id="1c883-173">customAttribute14</span></span> |
| <span data-ttu-id="1c883-174">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="1c883-174">extensionAttribute15</span></span> | <span data-ttu-id="1c883-175">customAttribute15</span><span class="sxs-lookup"><span data-stu-id="1c883-175">customAttribute15</span></span> |

## <a name="example"></a><span data-ttu-id="1c883-176">Пример</span><span class="sxs-lookup"><span data-stu-id="1c883-176">Example</span></span>

<span data-ttu-id="1c883-177">В следующем примере в карточку профиля добавляется первый настраиваемый атрибут расширения Azure AD, используемый для отображения имени **Cost center**.</span><span class="sxs-lookup"><span data-stu-id="1c883-177">The following example adds the first Azure AD custom extension attribute to the profile card, using the display name **Cost center**.</span></span> <span data-ttu-id="1c883-178">Для пользователей, выбравших в языковых настройках немецкий язык, отображаемым именем будет **Kostenstelle**.</span><span class="sxs-lookup"><span data-stu-id="1c883-178">For users that have set their language settings to German, the display name will be **Kostenstelle**.</span></span>

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

<span data-ttu-id="1c883-179">Если язык не поддерживается, имя свойства отображается с использованием значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1c883-179">If a language is not supported, the property name will be shown with the default value.</span></span>  

<span data-ttu-id="1c883-180">При успешном выполнении возвращается код отклика `201 OK` и объект **profileCardProperty** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c883-180">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="1c883-181">В этом примере вы можете предположить, что в карточке профиля отображается **Kostenstelle** для всех пользователей, выбравших в языковых настройках немецкий язык.</span><span class="sxs-lookup"><span data-stu-id="1c883-181">In this example you can assume that the profile card displays **Kostenstelle** for all users that have set their language settings to German on the profile card.</span></span> <span data-ttu-id="1c883-182">Для всех остальных пользователей в карточке профиля отображается **Cost center**.</span><span class="sxs-lookup"><span data-stu-id="1c883-182">For all other users, **Cost center** will be displayed on the profile card.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1c883-183">См. также</span><span class="sxs-lookup"><span data-stu-id="1c883-183">See also</span></span>

[<span data-ttu-id="1c883-184">Поиск идентификатора клиента Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1c883-184">Find your Microsoft 365 tenant ID</span></span>](/onedrive/find-your-office-365-tenant-id)

[<span data-ttu-id="1c883-185">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="1c883-185">onPremisesExtensionAttributes resource type</span></span>](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[<span data-ttu-id="1c883-186">Тип ресурса user</span><span class="sxs-lookup"><span data-stu-id="1c883-186">User resource type</span></span>](/graph/api/resources/user?view=graph-rest-beta)

[<span data-ttu-id="1c883-187">Песочница Graph</span><span class="sxs-lookup"><span data-stu-id="1c883-187">Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)

[<span data-ttu-id="1c883-188">Получение ресурса profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="1c883-188">Get profileCardProperty</span></span>](/graph/api/profilecardproperty-get?view=graph-rest-beta)
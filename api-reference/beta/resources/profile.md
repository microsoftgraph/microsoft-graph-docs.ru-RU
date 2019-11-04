---
title: Тип ресурса Profile
description: Представляет свойства, которые являются описательными для пользователя и представлены в общедоступных людях в Microsoft 365 и службах и возможностях сторонних производителей с помощью Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 367a2c556b560056bcab44e6c20ae7851e493e48
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950481"
---
# <a name="profile-resource-type"></a><span data-ttu-id="7c115-103">Тип ресурса Profile</span><span class="sxs-lookup"><span data-stu-id="7c115-103">profile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c115-104">Представляет свойства описания человека в клиенте.</span><span class="sxs-lookup"><span data-stu-id="7c115-104">Represents descriptive properties of a person in a tenant.</span></span> <span data-ttu-id="7c115-105">Эти свойства отображаются в общедоступных людях в Microsoft 365 и сторонних службах и возможностях в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7c115-105">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

## <a name="methods"></a><span data-ttu-id="7c115-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7c115-106">Methods</span></span>

| <span data-ttu-id="7c115-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7c115-107">Method</span></span>                                                                     | <span data-ttu-id="7c115-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c115-108">Return Type</span></span>                                                    | <span data-ttu-id="7c115-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7c115-109">Description</span></span>                                                                          |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------|
| [<span data-ttu-id="7c115-110">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="7c115-110">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="7c115-111">profile</span><span class="sxs-lookup"><span data-stu-id="7c115-111">profile</span></span>](profile.md)                                          | <span data-ttu-id="7c115-112">Чтение свойств и связей объекта Profile.</span><span class="sxs-lookup"><span data-stu-id="7c115-112">Read properties and relationships of profile object.</span></span>                                 |
| [<span data-ttu-id="7c115-113">Удаление профиля</span><span class="sxs-lookup"><span data-stu-id="7c115-113">Delete profile</span></span>](../api/profile-delete.md)                                         | <span data-ttu-id="7c115-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="7c115-114">None</span></span>                                                           | <span data-ttu-id="7c115-115">Удаление объекта **Profile** .</span><span class="sxs-lookup"><span data-stu-id="7c115-115">Delete a **profile** object.</span></span>                                                               |
| [<span data-ttu-id="7c115-116">Учетная запись списка</span><span class="sxs-lookup"><span data-stu-id="7c115-116">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="7c115-117">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-117">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="7c115-118">Получение коллекции объектов **усераккаунтинформатион** .</span><span class="sxs-lookup"><span data-stu-id="7c115-118">Get a **userAccountInformation** object collection.</span></span>                                      |
| [<span data-ttu-id="7c115-119">Создание Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="7c115-119">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="7c115-120">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="7c115-120">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="7c115-121">Создание нового **персонанниверсари** путем публикации в коллекции юбилеев.</span><span class="sxs-lookup"><span data-stu-id="7c115-121">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>           |
| [<span data-ttu-id="7c115-122">Список юбилеев</span><span class="sxs-lookup"><span data-stu-id="7c115-122">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="7c115-123">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-123">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="7c115-124">Получение коллекции объектов **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="7c115-124">Get a **personAnniversary** object collection.</span></span>                                           |
| [<span data-ttu-id="7c115-125">Создание Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="7c115-125">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="7c115-126">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="7c115-126">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="7c115-127">Создание нового **едукатионалактивити** путем отправки в коллекцию **едукатионалактивитиес** .</span><span class="sxs-lookup"><span data-stu-id="7c115-127">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="7c115-128">Список Едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="7c115-128">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="7c115-129">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-129">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="7c115-130">Получение коллекции объектов **едукатионалактивити** .</span><span class="sxs-lookup"><span data-stu-id="7c115-130">Get an **educationalActivity** object collection.</span></span>                                         |
| [<span data-ttu-id="7c115-131">Создание Итемемаил</span><span class="sxs-lookup"><span data-stu-id="7c115-131">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="7c115-132">итемемаил</span><span class="sxs-lookup"><span data-stu-id="7c115-132">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="7c115-133">Создание нового **итемемаил** путем отправки в коллекцию сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7c115-133">Create a new **itemEmail** by posting to the emails collection.</span></span>                          |
| [<span data-ttu-id="7c115-134">Список сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="7c115-134">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="7c115-135">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-135">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="7c115-136">Получение коллекции объектов **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="7c115-136">Get an **itemEmail** object collection.</span></span>                                                   |
| [<span data-ttu-id="7c115-137">Создание Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="7c115-137">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="7c115-138">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="7c115-138">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="7c115-139">Создание нового **персонинтерест** путем отправки в коллекцию интересов.</span><span class="sxs-lookup"><span data-stu-id="7c115-139">Create a new **personInterest** by posting to the interests collection.</span></span>                  |
| [<span data-ttu-id="7c115-140">Список интересов</span><span class="sxs-lookup"><span data-stu-id="7c115-140">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="7c115-141">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-141">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="7c115-142">Получение коллекции объектов **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="7c115-142">Get a **personInterest** object collection.</span></span>                                              |
| [<span data-ttu-id="7c115-143">Создание ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="7c115-143">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="7c115-144">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="7c115-144">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="7c115-145">Создание нового **лангуажепрофиЦиенци** путем публикации в коллекции Languages.</span><span class="sxs-lookup"><span data-stu-id="7c115-145">Create a new **languageProficiency** by posting to the languages collection.</span></span>             |
| [<span data-ttu-id="7c115-146">Список языков</span><span class="sxs-lookup"><span data-stu-id="7c115-146">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="7c115-147">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-147">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="7c115-148">Получение коллекции объектов **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="7c115-148">Get a **languageProficiency** object collection.</span></span>                                         |
| [<span data-ttu-id="7c115-149">Список имен</span><span class="sxs-lookup"><span data-stu-id="7c115-149">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="7c115-150">Коллекция [PersonName](personname.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-150">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="7c115-151">Получение коллекции объектов **PersonName** .</span><span class="sxs-lookup"><span data-stu-id="7c115-151">Get a **personName** object collection.</span></span>                                                  |
| [<span data-ttu-id="7c115-152">Создание personName</span><span class="sxs-lookup"><span data-stu-id="7c115-152">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="7c115-153">personName</span><span class="sxs-lookup"><span data-stu-id="7c115-153">personName</span></span>](personName.md)                                    | <span data-ttu-id="7c115-154">Создайте новый объект **PersonName** , отправив его в коллекцию Names.</span><span class="sxs-lookup"><span data-stu-id="7c115-154">Create a new **personName** object by posting to the names collection.</span></span>                   |
| [<span data-ttu-id="7c115-155">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="7c115-155">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="7c115-156">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-156">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="7c115-157">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="7c115-157">Get a **personWebsite** object collection.</span></span>                                               |
| [<span data-ttu-id="7c115-158">Создание Итемфоне</span><span class="sxs-lookup"><span data-stu-id="7c115-158">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="7c115-159">итемфоне</span><span class="sxs-lookup"><span data-stu-id="7c115-159">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="7c115-160">Создание нового Итемфоне путем публикации в коллекции phones.</span><span class="sxs-lookup"><span data-stu-id="7c115-160">Create a new itemPhone by posting to the phones collection.</span></span>                          |
| [<span data-ttu-id="7c115-161">Перечисление телефонов</span><span class="sxs-lookup"><span data-stu-id="7c115-161">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="7c115-162">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-162">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="7c115-163">Получение коллекции объектов **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="7c115-163">Get a **itemPhone** object collection.</span></span>                                                   |
| [<span data-ttu-id="7c115-164">Создание Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="7c115-164">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="7c115-165">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="7c115-165">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="7c115-166">Создание нового Воркпоситион путем отправки в коллекцию Positions.</span><span class="sxs-lookup"><span data-stu-id="7c115-166">Create a new workPosition by posting to the positions collection.</span></span>                    |
| [<span data-ttu-id="7c115-167">Позиции списка</span><span class="sxs-lookup"><span data-stu-id="7c115-167">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="7c115-168">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-168">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="7c115-169">Получение коллекции объектов **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="7c115-169">Get a **workPosition** object collection.</span></span>                                                |
| [<span data-ttu-id="7c115-170">Создание ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="7c115-170">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="7c115-171">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="7c115-171">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="7c115-172">Создание нового **прожектпартиЦипатион** путем публикации в коллекции проектов.</span><span class="sxs-lookup"><span data-stu-id="7c115-172">Create a new **projectParticipation** by posting to the projects collection.</span></span>             |
| [<span data-ttu-id="7c115-173">Список проектов</span><span class="sxs-lookup"><span data-stu-id="7c115-173">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="7c115-174">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-174">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="7c115-175">Получение коллекции объектов **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="7c115-175">Get a **projectParticipation** object collection.</span></span>                                        |
| [<span data-ttu-id="7c115-176">Создание СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="7c115-176">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="7c115-177">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="7c115-177">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="7c115-178">Создание нового **скиллпрофиЦиенци** путем публикации в коллекции навыков.</span><span class="sxs-lookup"><span data-stu-id="7c115-178">Create a new **skillProficiency** by posting to the skills collection.</span></span>                   |
| [<span data-ttu-id="7c115-179">Список навыков</span><span class="sxs-lookup"><span data-stu-id="7c115-179">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="7c115-180">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-180">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="7c115-181">Получение коллекции объектов **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="7c115-181">Get a **skillProficiency** object collection.</span></span>                                            |
| [<span data-ttu-id="7c115-182">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="7c115-182">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="7c115-183">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="7c115-183">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="7c115-184">Создайте новую **учетную запись** , разместив ее в коллекции учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7c115-184">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                    |
| [<span data-ttu-id="7c115-185">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="7c115-185">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="7c115-186">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-186">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="7c115-187">Получение коллекции объектов **учетных записей** .</span><span class="sxs-lookup"><span data-stu-id="7c115-187">Get a **webAccount** object collection.</span></span>                                                  |
| [<span data-ttu-id="7c115-188">Создание Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="7c115-188">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="7c115-189">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="7c115-189">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="7c115-190">Создание нового **персонвебсите** путем публикации в семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="7c115-190">Create a new **personWebsite** by posting to the websites collection.</span></span>                    |
| [<span data-ttu-id="7c115-191">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="7c115-191">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="7c115-192">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-192">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="7c115-193">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="7c115-193">Get a **personWebsite** object collection.</span></span>                                               |

## <a name="properties"></a><span data-ttu-id="7c115-194">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c115-194">Properties</span></span>

| <span data-ttu-id="7c115-195">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c115-195">Property</span></span>     | <span data-ttu-id="7c115-196">Тип</span><span class="sxs-lookup"><span data-stu-id="7c115-196">Type</span></span>        | <span data-ttu-id="7c115-197">Описание</span><span class="sxs-lookup"><span data-stu-id="7c115-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c115-198">id</span><span class="sxs-lookup"><span data-stu-id="7c115-198">id</span></span>            |<span data-ttu-id="7c115-199">String</span><span class="sxs-lookup"><span data-stu-id="7c115-199">String</span></span>       | <span data-ttu-id="7c115-200">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-200">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="7c115-201">Отношения</span><span class="sxs-lookup"><span data-stu-id="7c115-201">Relationships</span></span>

| <span data-ttu-id="7c115-202">Связь</span><span class="sxs-lookup"><span data-stu-id="7c115-202">Relationship</span></span>          | <span data-ttu-id="7c115-203">Тип</span><span class="sxs-lookup"><span data-stu-id="7c115-203">Type</span></span>                                                         | <span data-ttu-id="7c115-204">Описание</span><span class="sxs-lookup"><span data-stu-id="7c115-204">Description</span></span>         |
|:----------------------|:-------------------------------------------------------------|:--------------------|
|<span data-ttu-id="7c115-205">финансового</span><span class="sxs-lookup"><span data-stu-id="7c115-205">account</span></span>                |<span data-ttu-id="7c115-206">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-206">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="7c115-207">Представляет сведения, специально связанные с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c115-207">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="7c115-208">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-208">Read-only.</span></span> <span data-ttu-id="7c115-209">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-209">Nullable.</span></span>|
|<span data-ttu-id="7c115-210">годовщины</span><span class="sxs-lookup"><span data-stu-id="7c115-210">anniversaries</span></span>          |<span data-ttu-id="7c115-211">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-211">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="7c115-212">Представляет сведения о значимых датах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="7c115-212">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="7c115-213">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-213">Read-only.</span></span> <span data-ttu-id="7c115-214">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-214">Nullable.</span></span>|
|<span data-ttu-id="7c115-215">едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="7c115-215">educationalActivities</span></span>  |<span data-ttu-id="7c115-216">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-216">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="7c115-217">Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям.</span><span class="sxs-lookup"><span data-stu-id="7c115-217">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="7c115-218">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-218">Read-only.</span></span> <span data-ttu-id="7c115-219">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-219">Nullable.</span></span>|
|<span data-ttu-id="7c115-220">письма</span><span class="sxs-lookup"><span data-stu-id="7c115-220">emails</span></span>                 |<span data-ttu-id="7c115-221">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-221">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="7c115-222">Представляет подробные сведения об адресах электронной почты, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="7c115-222">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="7c115-223">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-223">Read-only.</span></span> <span data-ttu-id="7c115-224">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-224">Nullable.</span></span>|
|<span data-ttu-id="7c115-225">interests;</span><span class="sxs-lookup"><span data-stu-id="7c115-225">interests</span></span>              |<span data-ttu-id="7c115-226">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-226">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="7c115-227">Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.</span><span class="sxs-lookup"><span data-stu-id="7c115-227">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="7c115-228">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-228">Read-only.</span></span> <span data-ttu-id="7c115-229">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-229">Nullable.</span></span>|
|<span data-ttu-id="7c115-230">Языки</span><span class="sxs-lookup"><span data-stu-id="7c115-230">languages</span></span>              |<span data-ttu-id="7c115-231">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-231">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="7c115-232">Представляет подробные сведения о языках, добавленных пользователем в свой профиль.</span><span class="sxs-lookup"><span data-stu-id="7c115-232">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="7c115-233">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-233">Read-only.</span></span> <span data-ttu-id="7c115-234">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-234">Nullable.</span></span>|
|<span data-ttu-id="7c115-235">phones</span><span class="sxs-lookup"><span data-stu-id="7c115-235">phones</span></span>                 |<span data-ttu-id="7c115-236">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-236">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="7c115-237">Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="7c115-237">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="7c115-238">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-238">Read-only.</span></span> <span data-ttu-id="7c115-239">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-239">Nullable.</span></span>|
|<span data-ttu-id="7c115-240">расположен</span><span class="sxs-lookup"><span data-stu-id="7c115-240">positions</span></span>              |<span data-ttu-id="7c115-241">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-241">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="7c115-242">Представляет подробные сведения о должностных единицах, связанных с профилем пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c115-242">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="7c115-243">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-243">Read-only.</span></span> <span data-ttu-id="7c115-244">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-244">Nullable.</span></span>|
|<span data-ttu-id="7c115-245">projects</span><span class="sxs-lookup"><span data-stu-id="7c115-245">projects</span></span>               |<span data-ttu-id="7c115-246">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-246">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="7c115-247">Представляет подробные сведения о проектах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="7c115-247">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="7c115-248">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-248">Read-only.</span></span> <span data-ttu-id="7c115-249">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-249">Nullable.</span></span>|
|<span data-ttu-id="7c115-250">skills.</span><span class="sxs-lookup"><span data-stu-id="7c115-250">skills</span></span>                 |<span data-ttu-id="7c115-251">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-251">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="7c115-252">Представляет подробные сведения о навыках, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="7c115-252">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="7c115-253">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-253">Read-only.</span></span> <span data-ttu-id="7c115-254">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-254">Nullable.</span></span>|
|<span data-ttu-id="7c115-255">Учетные записи учетных записей</span><span class="sxs-lookup"><span data-stu-id="7c115-255">webAccounts</span></span>            |<span data-ttu-id="7c115-256">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-256">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="7c115-257">Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой профиль пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c115-257">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="7c115-258">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-258">Read-only.</span></span> <span data-ttu-id="7c115-259">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-259">Nullable.</span></span>|
|<span data-ttu-id="7c115-260">websites</span><span class="sxs-lookup"><span data-stu-id="7c115-260">websites</span></span>               |<span data-ttu-id="7c115-261">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="7c115-261">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="7c115-262">Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="7c115-262">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="7c115-263">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c115-263">Read-only.</span></span> <span data-ttu-id="7c115-264">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7c115-264">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c115-265">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c115-265">JSON representation</span></span>

<span data-ttu-id="7c115-266">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c115-266">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

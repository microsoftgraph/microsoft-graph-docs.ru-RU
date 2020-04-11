---
title: Тип ресурса Profile
description: Представляет свойства, которые являются описательными для пользователя и представлены в общедоступных людях в Microsoft 365 и службах и возможностях сторонних производителей с помощью Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8b398ee8b0dbe14570f4ae59c71372502f3d0565
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227709"
---
# <a name="profile-resource-type"></a><span data-ttu-id="c4015-103">Тип ресурса Profile</span><span class="sxs-lookup"><span data-stu-id="c4015-103">profile resource type</span></span>

<span data-ttu-id="c4015-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4015-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4015-105">Представляет свойства описания человека в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c4015-105">Represents descriptive properties of a person in a tenant.</span></span> <span data-ttu-id="c4015-106">Эти свойства отображаются в общедоступных людях в Microsoft 365 и сторонних службах и возможностях в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c4015-106">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

## <a name="methods"></a><span data-ttu-id="c4015-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c4015-107">Methods</span></span>

| <span data-ttu-id="c4015-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c4015-108">Method</span></span>                                                                     | <span data-ttu-id="c4015-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4015-109">Return Type</span></span>                                                    | <span data-ttu-id="c4015-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c4015-110">Description</span></span>                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [<span data-ttu-id="c4015-111">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="c4015-111">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="c4015-112">profile</span><span class="sxs-lookup"><span data-stu-id="c4015-112">profile</span></span>](profile.md)                                          | <span data-ttu-id="c4015-113">Чтение свойств и связей объекта Profile.</span><span class="sxs-lookup"><span data-stu-id="c4015-113">Read properties and relationships of profile object.</span></span>                                         |
| [<span data-ttu-id="c4015-114">Удаление профиля</span><span class="sxs-lookup"><span data-stu-id="c4015-114">Delete profile</span></span>](../api/profile-delete.md)                                 | <span data-ttu-id="c4015-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c4015-115">None</span></span>                                                           | <span data-ttu-id="c4015-116">Удаление объекта **Profile** .</span><span class="sxs-lookup"><span data-stu-id="c4015-116">Delete a **profile** object.</span></span>                                                                 |
| [<span data-ttu-id="c4015-117">Учетная запись списка</span><span class="sxs-lookup"><span data-stu-id="c4015-117">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="c4015-118">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-118">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="c4015-119">Получение коллекции объектов **усераккаунтинформатион** .</span><span class="sxs-lookup"><span data-stu-id="c4015-119">Get a **userAccountInformation** object collection.</span></span>                                          |
| [<span data-ttu-id="c4015-120">Создание Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="c4015-120">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="c4015-121">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="c4015-121">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="c4015-122">Создание нового **персонанниверсари** путем публикации в коллекции юбилеев.</span><span class="sxs-lookup"><span data-stu-id="c4015-122">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>               |
| [<span data-ttu-id="c4015-123">Список юбилеев</span><span class="sxs-lookup"><span data-stu-id="c4015-123">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="c4015-124">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-124">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="c4015-125">Получение коллекции объектов **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="c4015-125">Get a **personAnniversary** object collection.</span></span>                                               |
| [<span data-ttu-id="c4015-126">Создание Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="c4015-126">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="c4015-127">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="c4015-127">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="c4015-128">Создание нового **едукатионалактивити** путем отправки в коллекцию **едукатионалактивитиес** .</span><span class="sxs-lookup"><span data-stu-id="c4015-128">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="c4015-129">Список Едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="c4015-129">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="c4015-130">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-130">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="c4015-131">Получение коллекции объектов **едукатионалактивити** .</span><span class="sxs-lookup"><span data-stu-id="c4015-131">Get an **educationalActivity** object collection.</span></span>                                            |
| [<span data-ttu-id="c4015-132">Создание Итемемаил</span><span class="sxs-lookup"><span data-stu-id="c4015-132">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="c4015-133">итемемаил</span><span class="sxs-lookup"><span data-stu-id="c4015-133">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="c4015-134">Создание нового **итемемаил** путем отправки в коллекцию сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c4015-134">Create a new **itemEmail** by posting to the emails collection.</span></span>                              |
| [<span data-ttu-id="c4015-135">Список сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="c4015-135">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="c4015-136">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-136">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="c4015-137">Получение коллекции объектов **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="c4015-137">Get an **itemEmail** object collection.</span></span>                                                      |
| [<span data-ttu-id="c4015-138">Создание Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="c4015-138">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="c4015-139">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="c4015-139">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="c4015-140">Создание нового **персонинтерест** путем отправки в коллекцию интересов.</span><span class="sxs-lookup"><span data-stu-id="c4015-140">Create a new **personInterest** by posting to the interests collection.</span></span>                      |
| [<span data-ttu-id="c4015-141">Список интересов</span><span class="sxs-lookup"><span data-stu-id="c4015-141">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="c4015-142">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-142">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="c4015-143">Получение коллекции объектов **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="c4015-143">Get a **personInterest** object collection.</span></span>                                                  |
| [<span data-ttu-id="c4015-144">Создание ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c4015-144">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="c4015-145">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c4015-145">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="c4015-146">Создание нового **лангуажепрофиЦиенци** путем публикации в коллекции Languages.</span><span class="sxs-lookup"><span data-stu-id="c4015-146">Create a new **languageProficiency** by posting to the languages collection.</span></span>                 |
| [<span data-ttu-id="c4015-147">Список языков</span><span class="sxs-lookup"><span data-stu-id="c4015-147">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="c4015-148">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-148">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="c4015-149">Получение коллекции объектов **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="c4015-149">Get a **languageProficiency** object collection.</span></span>                                             |
| [<span data-ttu-id="c4015-150">Список имен</span><span class="sxs-lookup"><span data-stu-id="c4015-150">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="c4015-151">Коллекция [PersonName](personname.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-151">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="c4015-152">Получение коллекции объектов **PersonName** .</span><span class="sxs-lookup"><span data-stu-id="c4015-152">Get a **personName** object collection.</span></span>                                                      |
| [<span data-ttu-id="c4015-153">Создание personName</span><span class="sxs-lookup"><span data-stu-id="c4015-153">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="c4015-154">personName</span><span class="sxs-lookup"><span data-stu-id="c4015-154">personName</span></span>](personName.md)                                    | <span data-ttu-id="c4015-155">Создайте новый объект **PersonName** , отправив его в коллекцию Names.</span><span class="sxs-lookup"><span data-stu-id="c4015-155">Create a new **personName** object by posting to the names collection.</span></span>                       |
| [<span data-ttu-id="c4015-156">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="c4015-156">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="c4015-157">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-157">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="c4015-158">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="c4015-158">Get a **personWebsite** object collection.</span></span>                                                   |
| [<span data-ttu-id="c4015-159">Создание Итемфоне</span><span class="sxs-lookup"><span data-stu-id="c4015-159">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="c4015-160">итемфоне</span><span class="sxs-lookup"><span data-stu-id="c4015-160">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="c4015-161">Создание нового Итемфоне путем публикации в коллекции phones.</span><span class="sxs-lookup"><span data-stu-id="c4015-161">Create a new itemPhone by posting to the phones collection.</span></span>                                  |
| [<span data-ttu-id="c4015-162">Перечисление телефонов</span><span class="sxs-lookup"><span data-stu-id="c4015-162">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="c4015-163">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-163">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="c4015-164">Получение коллекции объектов **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="c4015-164">Get a **itemPhone** object collection.</span></span>                                                       |
| [<span data-ttu-id="c4015-165">Создание Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="c4015-165">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="c4015-166">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="c4015-166">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="c4015-167">Создание нового Воркпоситион путем отправки в коллекцию Positions.</span><span class="sxs-lookup"><span data-stu-id="c4015-167">Create a new workPosition by posting to the positions collection.</span></span>                            |
| [<span data-ttu-id="c4015-168">Позиции списка</span><span class="sxs-lookup"><span data-stu-id="c4015-168">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="c4015-169">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-169">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="c4015-170">Получение коллекции объектов **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="c4015-170">Get a **workPosition** object collection.</span></span>                                                    |
| [<span data-ttu-id="c4015-171">Создание ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="c4015-171">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="c4015-172">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="c4015-172">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="c4015-173">Создание нового **прожектпартиЦипатион** путем публикации в коллекции проектов.</span><span class="sxs-lookup"><span data-stu-id="c4015-173">Create a new **projectParticipation** by posting to the projects collection.</span></span>                 |
| [<span data-ttu-id="c4015-174">Список проектов</span><span class="sxs-lookup"><span data-stu-id="c4015-174">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="c4015-175">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-175">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="c4015-176">Получение коллекции объектов **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="c4015-176">Get a **projectParticipation** object collection.</span></span>                                            |
| [<span data-ttu-id="c4015-177">Создание СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c4015-177">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="c4015-178">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c4015-178">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="c4015-179">Создание нового **скиллпрофиЦиенци** путем публикации в коллекции навыков.</span><span class="sxs-lookup"><span data-stu-id="c4015-179">Create a new **skillProficiency** by posting to the skills collection.</span></span>                       |
| [<span data-ttu-id="c4015-180">Список навыков</span><span class="sxs-lookup"><span data-stu-id="c4015-180">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="c4015-181">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-181">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="c4015-182">Получение коллекции объектов **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="c4015-182">Get a **skillProficiency** object collection.</span></span>                                                |
| [<span data-ttu-id="c4015-183">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="c4015-183">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="c4015-184">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="c4015-184">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="c4015-185">Создайте новую **учетную запись** , разместив ее в коллекции учетных записей.</span><span class="sxs-lookup"><span data-stu-id="c4015-185">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                        |
| [<span data-ttu-id="c4015-186">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="c4015-186">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="c4015-187">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-187">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="c4015-188">Получение коллекции объектов **учетных записей** .</span><span class="sxs-lookup"><span data-stu-id="c4015-188">Get a **webAccount** object collection.</span></span>                                                      |
| [<span data-ttu-id="c4015-189">Создание Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="c4015-189">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="c4015-190">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="c4015-190">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="c4015-191">Создание нового **персонвебсите** путем публикации в семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="c4015-191">Create a new **personWebsite** by posting to the websites collection.</span></span>                        |
| [<span data-ttu-id="c4015-192">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="c4015-192">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="c4015-193">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-193">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="c4015-194">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="c4015-194">Get a **personWebsite** object collection.</span></span>                                                   |

## <a name="properties"></a><span data-ttu-id="c4015-195">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4015-195">Properties</span></span>

| <span data-ttu-id="c4015-196">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4015-196">Property</span></span>     | <span data-ttu-id="c4015-197">Тип</span><span class="sxs-lookup"><span data-stu-id="c4015-197">Type</span></span>        | <span data-ttu-id="c4015-198">Описание</span><span class="sxs-lookup"><span data-stu-id="c4015-198">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c4015-199">id</span><span class="sxs-lookup"><span data-stu-id="c4015-199">id</span></span>            |<span data-ttu-id="c4015-200">String</span><span class="sxs-lookup"><span data-stu-id="c4015-200">String</span></span>       | <span data-ttu-id="c4015-201">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-201">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="c4015-202">Отношения</span><span class="sxs-lookup"><span data-stu-id="c4015-202">Relationships</span></span>

| <span data-ttu-id="c4015-203">Связь</span><span class="sxs-lookup"><span data-stu-id="c4015-203">Relationship</span></span>          | <span data-ttu-id="c4015-204">Тип</span><span class="sxs-lookup"><span data-stu-id="c4015-204">Type</span></span>                                                         | <span data-ttu-id="c4015-205">Описание</span><span class="sxs-lookup"><span data-stu-id="c4015-205">Description</span></span>                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="c4015-206">финансового</span><span class="sxs-lookup"><span data-stu-id="c4015-206">account</span></span>                |<span data-ttu-id="c4015-207">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-207">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="c4015-208">Представляет сведения, специально связанные с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4015-208">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="c4015-209">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-209">Read-only.</span></span> <span data-ttu-id="c4015-210">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-210">Nullable.</span></span>                                                             |
|<span data-ttu-id="c4015-211">годовщины</span><span class="sxs-lookup"><span data-stu-id="c4015-211">anniversaries</span></span>          |<span data-ttu-id="c4015-212">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-212">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="c4015-213">Представляет сведения о значимых датах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c4015-213">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="c4015-214">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-214">Read-only.</span></span> <span data-ttu-id="c4015-215">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-215">Nullable.</span></span>                                                      |
|<span data-ttu-id="c4015-216">едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="c4015-216">educationalActivities</span></span>  |<span data-ttu-id="c4015-217">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-217">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="c4015-218">Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям.</span><span class="sxs-lookup"><span data-stu-id="c4015-218">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="c4015-219">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-219">Read-only.</span></span> <span data-ttu-id="c4015-220">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-220">Nullable.</span></span>|
|<span data-ttu-id="c4015-221">письма</span><span class="sxs-lookup"><span data-stu-id="c4015-221">emails</span></span>                 |<span data-ttu-id="c4015-222">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-222">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="c4015-223">Представляет подробные сведения об адресах электронной почты, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c4015-223">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="c4015-224">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-224">Read-only.</span></span> <span data-ttu-id="c4015-225">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-225">Nullable.</span></span>                                           |
|<span data-ttu-id="c4015-226">interests;</span><span class="sxs-lookup"><span data-stu-id="c4015-226">interests</span></span>              |<span data-ttu-id="c4015-227">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-227">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="c4015-228">Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c4015-228">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="c4015-229">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-229">Read-only.</span></span> <span data-ttu-id="c4015-230">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-230">Nullable.</span></span>                |
|<span data-ttu-id="c4015-231">Языки</span><span class="sxs-lookup"><span data-stu-id="c4015-231">languages</span></span>              |<span data-ttu-id="c4015-232">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-232">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="c4015-233">Представляет подробные сведения о языках, добавленных пользователем в свой профиль.</span><span class="sxs-lookup"><span data-stu-id="c4015-233">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="c4015-234">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-234">Read-only.</span></span> <span data-ttu-id="c4015-235">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-235">Nullable.</span></span>                                   |
|<span data-ttu-id="c4015-236">phones</span><span class="sxs-lookup"><span data-stu-id="c4015-236">phones</span></span>                 |<span data-ttu-id="c4015-237">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-237">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="c4015-238">Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c4015-238">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="c4015-239">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-239">Read-only.</span></span> <span data-ttu-id="c4015-240">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-240">Nullable.</span></span>                           |
|<span data-ttu-id="c4015-241">расположен</span><span class="sxs-lookup"><span data-stu-id="c4015-241">positions</span></span>              |<span data-ttu-id="c4015-242">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-242">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="c4015-243">Представляет подробные сведения о должностных единицах, связанных с профилем пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4015-243">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="c4015-244">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-244">Read-only.</span></span> <span data-ttu-id="c4015-245">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-245">Nullable.</span></span>                                    |
|<span data-ttu-id="c4015-246">projects</span><span class="sxs-lookup"><span data-stu-id="c4015-246">projects</span></span>               |<span data-ttu-id="c4015-247">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-247">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="c4015-248">Представляет подробные сведения о проектах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c4015-248">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="c4015-249">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-249">Read-only.</span></span> <span data-ttu-id="c4015-250">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-250">Nullable.</span></span>                                                    |
|<span data-ttu-id="c4015-251">skills.</span><span class="sxs-lookup"><span data-stu-id="c4015-251">skills</span></span>                 |<span data-ttu-id="c4015-252">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-252">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="c4015-253">Представляет подробные сведения о навыках, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c4015-253">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="c4015-254">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-254">Read-only.</span></span> <span data-ttu-id="c4015-255">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-255">Nullable.</span></span>                                  |
|<span data-ttu-id="c4015-256">Учетные записи учетных записей</span><span class="sxs-lookup"><span data-stu-id="c4015-256">webAccounts</span></span>            |<span data-ttu-id="c4015-257">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-257">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="c4015-258">Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой профиль пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4015-258">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="c4015-259">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-259">Read-only.</span></span> <span data-ttu-id="c4015-260">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-260">Nullable.</span></span>                               |
|<span data-ttu-id="c4015-261">websites</span><span class="sxs-lookup"><span data-stu-id="c4015-261">websites</span></span>               |<span data-ttu-id="c4015-262">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="c4015-262">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="c4015-263">Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c4015-263">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="c4015-264">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4015-264">Read-only.</span></span> <span data-ttu-id="c4015-265">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4015-265">Nullable.</span></span>                                |

## <a name="json-representation"></a><span data-ttu-id="c4015-266">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4015-266">JSON representation</span></span>

<span data-ttu-id="c4015-267">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4015-267">The following is a JSON representation of the resource.</span></span>

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

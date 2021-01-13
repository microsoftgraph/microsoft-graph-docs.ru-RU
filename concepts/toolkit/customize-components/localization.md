---
title: Локализация компонентов Microsoft Graph Toolkit
description: Используйте LocalizationHelper для локализации компонентов Microsoft Graph Toolkit.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 3ac9f3fe5dedeb4e1793a589778242486f3b0070
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660095"
---
# <a name="localizing-the-microsoft-graph-toolkit-components"></a><span data-ttu-id="b0b79-103">Локализация компонентов Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="b0b79-103">Localizing the Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="b0b79-104">Локализация — это важный аспект разработки приложений для поддержки пользователей с разными языковыми требованиями по всему миру.</span><span class="sxs-lookup"><span data-stu-id="b0b79-104">Localization is a important aspect of application development to support users with various language requirements globally.</span></span>

<span data-ttu-id="b0b79-105">Чтобы пользовательский интерфейс отражал целевой язык, вы можете локализовать компоненты Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="b0b79-105">You can localize the Microsoft Graph Toolkit components to ensure that the UI reflects the target language.</span></span>

## <a name="use-localizationhelper-to-add-localized-strings"></a><span data-ttu-id="b0b79-106">Использование LocalizationHelper для добавления локализованных строк</span><span class="sxs-lookup"><span data-stu-id="b0b79-106">Use LocalizationHelper to add localized strings</span></span>

<span data-ttu-id="b0b79-107">В наборе средств Toolkit отсутствует локализация всех строк, но вы можете указывать собственные локализованные строки и управлять различными языками с помощью того же процесса, который применяется для локализации приложения.</span><span class="sxs-lookup"><span data-stu-id="b0b79-107">All strings in the toolkit are not localized, but you can provide your own localized strings and manage different languages through the same process you use for localizing your app.</span></span> <span data-ttu-id="b0b79-108">Чтобы облегчить локализацию, набор средств Toolkit предоставляет статический класс `LocalizationHelper`.</span><span class="sxs-lookup"><span data-stu-id="b0b79-108">To facilitate localization, the toolkit exposes the `LocalizationHelper` static class.</span></span>

<span data-ttu-id="b0b79-109">В примере ниже показано, как локализовать несколько компонентов.</span><span class="sxs-lookup"><span data-stu-id="b0b79-109">The following example shows how to localize several components.</span></span>

```ts
import { LocalizationHelper } from "@microsoft/mgt";

LocalizationHelper.strings = {
  noResultsFound: "لم نجد أي قنوات",
  _components: {
    "login": {
      signInLinkSubtitle: "login",
      signOutLinkSubtitle: "خروج",
    },
    "people-picker": {
      inputPlaceholderText: "ابدأ في كتابة الاسم",
      noResultsFound: "لم نجد أي قنوات", //collision with global defined noResultsFound will overwrite with local result
      loadingMessage: "...جار التحميل",
    },
    "teams-channel-picker": {
      inputPlaceholderText: "حدد قناة",
      noResultsFound: "local NoResultsFound Example",
      // loadingMessage: is default string "Loading..." for this example since not defined globally or locally
    },
    "tasks": {
      removeTaskSubtitle: "delete",
      cancelNewTaskSubtitle: "canceltest",
      newTaskPlaceholder: "newTaskTest",
      addTaskButtonSubtitle: "addme",
    },
    "person-card": {
      sendEmailLinkSubtitle: "ارسل بريد الكتروني",
      startChatLinkSubtitle: "ابدأ الدردشة",
      showMoreSectionButton: "أظهر المزيد", // global declaration
    },
    "person-card-contact": {
      contactSectionTitle: "اتصل",
    },
    "person-card-organization": {
      reportsToSectionTitle: "تقارير ل",
      directReportsSectionTitle: "تقارير مباشرة",
      organizationSectionTitle: "منظمة",
      youWorkWithSubSectionTitle: "انت تعمل مع",
      userWorksWithSubSectionTitle: "يعمل مع",
    },
  },
};
```

<span data-ttu-id="b0b79-110">При назначении свойства `strings` все компоненты автоматически получат новые строки и для них будет выполнен повторный рендеринг, что позволяет динамически изменять строки.</span><span class="sxs-lookup"><span data-stu-id="b0b79-110">When the `strings` property is assigned, all components will automatically pick up the new strings and re-render, allowing you to change strings dynamically.</span></span> 

<span data-ttu-id="b0b79-111">Строки можно задать на глобальном уровне или на уровне компонента (с помощью свойства `_components:`).</span><span class="sxs-lookup"><span data-stu-id="b0b79-111">The strings can be set at a global level or per component (with the `_components:` property).</span></span>

## <a name="strings"></a><span data-ttu-id="b0b79-112">Строки</span><span class="sxs-lookup"><span data-stu-id="b0b79-112">Strings</span></span>

### <a name="login"></a><span data-ttu-id="b0b79-113">Вход</span><span class="sxs-lookup"><span data-stu-id="b0b79-113">Login</span></span>

```ts
{
  signInLinkSubtitle: 'Sign In',
  signOutLinkSubtitle: 'Sign Out'
}
```

### <a name="people-picker"></a><span data-ttu-id="b0b79-114">Выбор людей</span><span class="sxs-lookup"><span data-stu-id="b0b79-114">People-Picker</span></span>

```ts
{
  inputPlaceholderText: 'Start typing a name',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="teams-channel-picker"></a><span data-ttu-id="b0b79-115">Средство выбора каналов Teams</span><span class="sxs-lookup"><span data-stu-id="b0b79-115">Teams-Channel-Picker</span></span>

```ts
{
  inputPlaceholderText: 'Select a channel',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="tasks"></a><span data-ttu-id="b0b79-116">Задачи</span><span class="sxs-lookup"><span data-stu-id="b0b79-116">Tasks</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="tasks-base"></a><span data-ttu-id="b0b79-117">Основные задачи</span><span class="sxs-lookup"><span data-stu-id="b0b79-117">Tasks-Base</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="todo"></a><span data-ttu-id="b0b79-118">To Do</span><span class="sxs-lookup"><span data-stu-id="b0b79-118">Todo</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="person-card"></a><span data-ttu-id="b0b79-119">Карточка контакта</span><span class="sxs-lookup"><span data-stu-id="b0b79-119">Person-Card</span></span>

```ts
{
  sendEmailLinkSubtitle: 'Send email',
  startChatLinkSubtitle: 'Start chat',
  showMoreSectionButton: 'Show more'
}
```

### <a name="person-card-contact"></a><span data-ttu-id="b0b79-120">Контактные данные карточки контакта</span><span class="sxs-lookup"><span data-stu-id="b0b79-120">Person-Card-Contact</span></span>

```ts
{
  contactSectionTitle: "Contact";
}
```

### <a name="person-card-organization"></a><span data-ttu-id="b0b79-121">Организация карточки контакта</span><span class="sxs-lookup"><span data-stu-id="b0b79-121">Person-Card-Organization</span></span>

```ts
{
  reportsToSectionTitle: 'Reports to',
  directReportsSectionTitle: 'Direct reports',
  organizationSectionTitle: 'Organization',
  youWorkWithSubSectionTitle: 'You work with',
  userWorksWithSubSectionTitle: 'works with'
}
```

### <a name="person-card-messages"></a><span data-ttu-id="b0b79-122">Сообщения карточки контакта</span><span class="sxs-lookup"><span data-stu-id="b0b79-122">Person-Card-Messages</span></span>

```ts
{
  emailsSectionTitle: "Emails";
}
```

### <a name="person-card-files"></a><span data-ttu-id="b0b79-123">Файлы карточки контакта</span><span class="sxs-lookup"><span data-stu-id="b0b79-123">Person-Card-Files</span></span>

```ts
{
  filesSectionTitle: 'Files',
  sharedTextSubtitle: 'Shared'
}
```

### <a name="person-card-profile"></a><span data-ttu-id="b0b79-124">Профиль карточки контакта</span><span class="sxs-lookup"><span data-stu-id="b0b79-124">Person-Card-Profile</span></span>

```ts
{
  SkillsAndExperienceSectionTitle: 'Skills & Experience',
  AboutCompactSectionTitle: 'About',
  SkillsSubSectionTitle: 'Skills',
  LanguagesSubSectionTitle: 'Languages',
  WorkExperienceSubSectionTitle: 'Work Experience',
  EducationSubSectionTitle: 'Education',
  professionalInterestsSubSectionTitle: 'Professional Interests',
  personalInterestsSubSectionTitle: 'Personal Interests',
  birthdaySubSectionTitle: 'Birthday',
  currentYearSubtitle: 'Current'
}
```

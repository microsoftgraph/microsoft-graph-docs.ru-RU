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
# <a name="localizing-the-microsoft-graph-toolkit-components"></a>Локализация компонентов Microsoft Graph Toolkit

Локализация — это важный аспект разработки приложений для поддержки пользователей с разными языковыми требованиями по всему миру.

Чтобы пользовательский интерфейс отражал целевой язык, вы можете локализовать компоненты Microsoft Graph Toolkit.

## <a name="use-localizationhelper-to-add-localized-strings"></a>Использование LocalizationHelper для добавления локализованных строк

В наборе средств Toolkit отсутствует локализация всех строк, но вы можете указывать собственные локализованные строки и управлять различными языками с помощью того же процесса, который применяется для локализации приложения. Чтобы облегчить локализацию, набор средств Toolkit предоставляет статический класс `LocalizationHelper`.

В примере ниже показано, как локализовать несколько компонентов.

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

При назначении свойства `strings` все компоненты автоматически получат новые строки и для них будет выполнен повторный рендеринг, что позволяет динамически изменять строки. 

Строки можно задать на глобальном уровне или на уровне компонента (с помощью свойства `_components:`).

## <a name="strings"></a>Строки

### <a name="login"></a>Вход

```ts
{
  signInLinkSubtitle: 'Sign In',
  signOutLinkSubtitle: 'Sign Out'
}
```

### <a name="people-picker"></a>Выбор людей

```ts
{
  inputPlaceholderText: 'Start typing a name',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="teams-channel-picker"></a>Средство выбора каналов Teams

```ts
{
  inputPlaceholderText: 'Select a channel',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="tasks"></a>Задачи

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="tasks-base"></a>Основные задачи

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="todo"></a>To Do

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="person-card"></a>Карточка контакта

```ts
{
  sendEmailLinkSubtitle: 'Send email',
  startChatLinkSubtitle: 'Start chat',
  showMoreSectionButton: 'Show more'
}
```

### <a name="person-card-contact"></a>Контактные данные карточки контакта

```ts
{
  contactSectionTitle: "Contact";
}
```

### <a name="person-card-organization"></a>Организация карточки контакта

```ts
{
  reportsToSectionTitle: 'Reports to',
  directReportsSectionTitle: 'Direct reports',
  organizationSectionTitle: 'Organization',
  youWorkWithSubSectionTitle: 'You work with',
  userWorksWithSubSectionTitle: 'works with'
}
```

### <a name="person-card-messages"></a>Сообщения карточки контакта

```ts
{
  emailsSectionTitle: "Emails";
}
```

### <a name="person-card-files"></a>Файлы карточки контакта

```ts
{
  filesSectionTitle: 'Files',
  sharedTextSubtitle: 'Shared'
}
```

### <a name="person-card-profile"></a>Профиль карточки контакта

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

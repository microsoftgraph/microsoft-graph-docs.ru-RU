---
title: Локализация компонентов Microsoft Graph Toolkit
description: Используйте LocalizationHelper для локализации компонентов Microsoft Graph Toolkit.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 934873a6695ce2e858173e0a8f965a7762805c76
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589235"
---
# <a name="localizing-the-microsoft-graph-toolkit-components"></a>Локализация компонентов Microsoft Graph Toolkit

Локализация является важным аспектом разработки приложений для поддержки пользователей с различными языковыми требованиями во всем мире.

Чтобы пользовательский интерфейс отражал целевой язык, вы можете локализовать компоненты Microsoft Graph Toolkit.

## <a name="use-localizationhelper-to-add-localized-strings"></a>Использование LocalizationHelper для добавления локализованных строк

Ни одна из строк в наборе инструментов не локализована, но вы можете предоставить собственные локализованные строки и управлять различными языками с помощью того же процесса, который используется для локализации приложения. Чтобы облегчить локализацию, набор средств Toolkit предоставляет статический класс `LocalizationHelper`.

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
      noResultsFound: "لم نجد أي قنوات", // will overwrite globally defined noResultsFound in people-picker component
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
      showExpandedDetailsButton: 'Show expanded details',
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

При присвоении `strings` `LocalizationHelper` свойству все компоненты автоматически подбирают новые строки и повторно отрисовку, что позволяет динамически изменять строки. 

Строки можно задать на глобальном уровне или на уровне компонента (с помощью свойства `_components:`).

## <a name="strings"></a>Строки

### <a name="login"></a>Вход

```ts
"login": {
  signInLinkSubtitle: "Sign In",
  signOutLinkSubtitle: "Sign Out"
}
```

### <a name="people-picker"></a>Выбор людей

```ts
"people-picker": {
  inputPlaceholderText: "Start typing a name",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="teams-channel-picker"></a>Средство выбора каналов Teams

```ts
"teams-channel-picker": {
  inputPlaceholderText: "Select a channel",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="tasks"></a>Задачи

```ts
"tasks": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="tasks-base"></a>Основные задачи

```ts
"tasks-base": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="todo"></a>To Do

```ts
"todo": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="person-card"></a>Карточка контакта

```ts
"person-card": {
  sendEmailLinkSubtitle: "Send email",
  startChatLinkSubtitle: "Start chat",
  showMoreSectionButton: "Show more"
}
```

### <a name="person-card-contact"></a>Контактные данные карточки контакта

```ts
"person-card-contact": {
  contactSectionTitle: "Contact"
}
```

### <a name="person-card-organization"></a>Организация карточки контакта

```ts
"person-card-organization": {
  reportsToSectionTitle: "Reports to",
  directReportsSectionTitle: "Direct reports",
  organizationSectionTitle: "Organization",
  youWorkWithSubSectionTitle: "You work with",
  userWorksWithSubSectionTitle: "works with"
}
```

### <a name="person-card-messages"></a>Сообщения карточки контакта

```ts
"person-card-messages": {
  emailsSectionTitle: "Emails"
}
```

### <a name="person-card-files"></a>Файлы карточки контакта

```ts
"person-card-files": {
  filesSectionTitle: "Files",
  sharedTextSubtitle: "Shared"
}
```

### <a name="person-card-profile"></a>Профиль карточки контакта

```ts
"person-card-profile": {
  SkillsAndExperienceSectionTitle: "Skills & Experience",
  AboutCompactSectionTitle: "About",
  SkillsSubSectionTitle: "Skills",
  LanguagesSubSectionTitle: "Languages",
  WorkExperienceSubSectionTitle: "Work Experience",
  EducationSubSectionTitle: "Education",
  professionalInterestsSubSectionTitle: "Professional Interests",
  personalInterestsSubSectionTitle: "Personal Interests",
  birthdaySubSectionTitle: "Birthday",
  currentYearSubtitle: "Current"
}
```

### <a name="file"></a>File

```ts
'file': {
  modifiedSubtitle: 'Modified',
  sizeSubtitle: 'Size'
};
```

### <a name="file-list"></a>File-List

```ts
"file-list": {
  showMoreSubtitle: 'Show more items'
}
```

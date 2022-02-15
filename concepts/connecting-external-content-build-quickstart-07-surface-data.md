---
ms.localizationpriority: medium
ms.openlocfilehash: 04ba810183228e3834069d9bfa620fe3c71fdb12
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805371"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

Создайте вертикали поиска и типы результатов для настройки результатов поиска в Microsoft SharePoint, Microsoft Office и Поиск (Майкрософт) в Bing, чтобы пользователям было проще находить сведения, которые они могут видеть.

## <a name="create-a-vertical"></a>Создание вертикали

Чтобы создать и включить вертикаль поиска на уровне организации, вопишитесь в [](https://admin.microsoft.com/) центр Microsoft 365 Admin с помощью роли глобального администратора и сделайте следующее:

1. Перейдите **Параметры** >  **Search &** **intelligenceCustomizations** > .
2. Перейдите **в Vertical** и нажмите **кнопку Добавить** .
3. Укай следующие сведения:
  * **Назови вертикаль:** Части прибора.

   ![Снимок экрана раздела "Имя вертикали"](images/connectors-images/build11.png)

  * **Источник контента**. Соединитектор, созданный с помощью приложения. (Запас частей)

   ![Снимок экрана раздела "Источник контента"](images/connectors-images/build12.png)

  * **Добавление запроса**. Оставьте пустым.

   ![Снимок экрана раздела "Добавление запроса"](images/connectors-images/build13.png)

  * **Фильтры**. Оставьте пустым.

   ![Снимок экрана раздела "Фильтры"](images/connectors-images/build14.png)

## <a name="create-a-result-type"></a>Создание типа результатов

Чтобы создать тип результатов:

1. Перейдите **Параметры** >  **Search &** **intelligenceCustomizations** > .
2. Перейдите на **вкладку типа результатов** и нажмите **кнопку Добавить** .
3. Укай следующие сведения:

  * **Имя**: Бытовая часть

   ![Снимок экрана раздела "Имя типа результата"](images/connectors-images/build15.png)

  * **Источник контента**. Соединитектор, созданный в приложении.

   ![Снимок экрана раздела "Выбор источника контента"](images/connectors-images/build16.png)

  * **Правила**: Нет

   ![Снимок экрана раздела "Набор правил"](images/connectors-images/build17.png)

  * Введите содержимое [result-type.json в](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) текстовый ящик конструктора макета.

   ![Снимок экрана раздела "Макет дизайна"](images/connectors-images/build18.png)

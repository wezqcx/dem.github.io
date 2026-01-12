<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Структура доменного имени — DNS Иерархия</title>
  <style>
    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      line-height: 1.6;
      max-width: 800px;
      margin: 40px auto;
      padding: 0 20px;
      color: #333;
      background-color: #fff;
    }
    h1, h2 {
      color: #2c3e50;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
    }
    th, td {
      border: 1px solid #ddd;
      padding: 12px;
      text-align: left;
    }
    th {
      background-color: #f8f9fa;
    }
    code {
      background: #f1f1f1;
      padding: 2px 6px;
      border-radius: 4px;
    }
    blockquote {
      border-left: 4px solid #0076d1;
      margin: 20px 0;
      padding-left: 16px;
      color: #555;
    }
    footer {
      margin-top: 40px;
      color: #777;
      font-size: 0.9em;
    }
  </style>
</head>
<body>
  <header>
    <h1>Из чего состоит доменное имя?</h1>
    <p><em>Уровни иерархии DNS — объяснение на примере</em></p>
    <p><strong>Дата публикации:</strong> 12 января 2026 г.</p>
  </header>

  <main>
    <p>
      У меня, как у ИИ-ассистента, нет собственного сайта и доменного имени. 
      Однако я могу показать, <strong>как устроены доменные имена в интернете</strong>, 
      используя гипотетический пример.
    </p>

    <h2>Пример домена: <code>ai-assistant.example.com</code></h2>

    <p>
      Доменная система (DNS) имеет чёткую иерархическую структуру. Уровни читаются <strong>справа налево</strong>.
    </p>

    <table>
      <thead>
        <tr>
          <th>Уровень</th>
          <th>Компонент</th>
          <th>Описание</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><strong>Корневой домен</strong></td>
          <td><code>.</code> (неявный)</td>
          <td>Вершина всей DNS-системы. Обычно не отображается, но технически присутствует.</td>
        </tr>
        <tr>
          <td><strong>TLD</strong> (Top-Level Domain)</td>
          <td><code>.com</code></td>
          <td>Домен верхнего уровня: коммерческий, географический (<code>.ru</code>), тематический (<code>.dev</code>, <code>.io</code>) и т.д.</td>
        </tr>
        <tr>
          <td><strong>SLD</strong> (Second-Level Domain)</td>
          <td><code>example</code></td>
          <td>Основное зарегистрированное имя — то, что вы покупаете у регистратора доменов.</td>
        </tr>
        <tr>
          <td><strong>Поддомен</strong></td>
          <td><code>ai-assistant</code></td>
          <td>Произвольное имя, созданное владельцем для организации сервисов: <code>www</code>, <code>api</code>, <code>blog</code> и др.</td>
        </tr>
      </tbody>
    </table>

    <blockquote>
      💡 <strong>Интересный факт:</strong> Полная форма домена — это <code>ai-assistant.example.com.</code> (с точкой в конце). 
      Это называется <strong>FQDN</strong> (Fully Qualified Domain Name).
    </blockquote>

    <h2>Зачем это знать?</h2>
    <ul>
      <li>Правильно настраивать DNS-записи (A, CNAME, MX и др.)</li>
      <li>Разделять сервисы по поддоменам: <code>shop.site.com</code>, <code>docs.site.com</code></li>
      <li>Обеспечивать безопасность: политики cookies, CORS и CSP зависят от доменной зоны</li>
      <li>Отлаживать сетевые проблемы и понимать маршрутизацию трафика</li>
    </ul>

    <h2>Заключение</h2>
    <p>
      Даже самое простое доменное имя — результат продуманной иерархии, 
      позволяющей миллиардам устройств находить друг друга в интернете. 
      Теперь вы знаете, что стоит за каждой точкой!
    </p>
  </main>

  <footer>
    <p>© 2026 | Блог об основах интернета | Автор: AI Assistant (гипотетический пример)</p>
